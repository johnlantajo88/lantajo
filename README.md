
public class Main {


    public static String concatenateStrings(String str1, String str2, String str3, String str4, String str5) {
        int len1 = str1.length();
        int len2 = str2.length();
        int len3 = str3.length();  // Fixed typo: 'lenght' -> 'length'
        int len4 = str4.length();  // Fixed typo: 'lenght' -> 'length'
        int len5 = str5.length();
        
        // Create a char array large enough to hold all characters from the five strings
        char[] result = new char[len1 + len2 + len3 + len4 + len5];

        int i = 0;
        // Copy characters from str1
        while (i < len1) {
            result[i] = str1.charAt(i);
            i++;
        }

        // Copy characters from str2
        int j = 0;
        while (i < len1 + len2) {
            result[i] = str2.charAt(j);
            i++;
            j++;
        }

        // Copy characters from str3
        j = 0;
        while (i < len1 + len2 + len3) {
            result[i] = str3.charAt(j);
            i++;
            j++;
        }

        // Copy characters from str4
        j = 0;
        while (i < len1 + len2 + len3 + len4) {
            result[i] = str4.charAt(j);
            i++;
            j++;
        }

        // Copy characters from str5
        j = 0;
        while (i < len1 + len2 + len3 + len4 + len5) {
            result[i] = str5.charAt(j);
            i++;
            j++;
        }

        // Return the concatenated string
        return new String(result);
    }

    public static void main(String[] args) {
        String str1 = "John";
        String str2 = "Benedict";
        String str3 = "Lovitos";
        String str4 = "Lantajo";
        String str5 = "Llagas";
        
        // Call the method with all 5 strings
        String concatenatedString = concatenateStrings(str1, str2, str3, str4, str5);
        System.out.println("Concatenated string: " + concatenatedString);
    }
}
