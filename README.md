# TASK 3
import java.io.BufferedReader; 
import java.io.InputStreamReader; 
import java.net.HttpURLConnection; 
import java.net.URL; 
import java.util.Scanner; 
import org.json.JSONObject; 
public class CurrencyConverter { 
private static final String API_KEY = "YOUR_API_KEY";   
private static final String API_URL = "https://v6.exchangerate-api.com/v6/%s/latest/%s";   
public static void main(String[] args) { 
Scanner scanner = new Scanner(System.in); 
System.out.print("Enter the base currency (e.g., USD, EUR): "); 
        String baseCurrency = scanner.nextLine().toUpperCase(); 
         
        System.out.print("Enter the target currency (e.g., USD, EUR): "); 
        String targetCurrency = scanner.nextLine().toUpperCase(); 
         
        System.out.print("Enter the amount to convert: "); 
        double amount = scanner.nextDouble(); 
         
        try { 
            double exchangeRate = getExchangeRate(baseCurrency, targetCurrency); 
             
        }
        }
