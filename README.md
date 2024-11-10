# JavaSharingSession
## Apa itu Java
###
## Mari kita mulai
- Install
- Create Project
- Syntax
    ```
    public class Main {
      public static void main(String[] args) {
        System.out.println("Hello World");
      }
    }
  ```
- Tipe Data
    - Numeric
      - primitve : ```int, long, float, double, char, short, byte, boolean ```
      - non-primitve: ```String, Integer, Long, Float, Double, Array, Class```
    - Non-Numeric
      ```String dan Character```
    - Collection
      ```Array```
- Variable
    - final
      ```
        final String company = "Allianz";
      ```
    - static
      ```
        static String company = "Allianz";
      ```
    - private
      ```
        private String company = "Allianz";
      ```
    - public
        ```
        public String company = "Allianz";
      ```
    - Volatile
      ```
        volatile String company = "Allianz";
      ```
- Operator
  ```
   + - * / % Math.pow(bilangan, pangkat) \
  ```
- IF
- Switch
- For Loop
- While Loop
- I/O
  - File
    - Read File
      ```
	    private void useBuffer(){
			String namafile = "file.txt";
			File file = new File(namafile);
			if(file.exists()) {
				FileReader fileReader = new FileReader(file);
				BufferedReader buffer = new BufferedReader(fileReader);
				String tmp = "";
				String result = "";
				while((tmp=buffer.readLine())!= null) {
					result += tmp +"\n";
				}
				System.out.println(result);
			}
	    }

	    public void useScanner() {
		    try {
		      File file = new File("file.txt");
		      Scanner scanner = new Scanner(file);
		      String result = null;
		      while (scanner.hasNextLine()) {
		        result += scanner.nextLine()+"\n";
		      }
		      System.out.println(result);
		      scanner.close();
		    } catch (FileNotFoundException e) {
		      e.printStackTrace();
		    }
	    }
	    public void useFileReader() throws IOException {
			FileReader fr = new FileReader("file.txt");
		    int i;
		    String result = "";
		    while ((i = fr.read()) != -1) {
		    	System.out.print((char)i);
		    }
		    
	    }
      ```
    - Write File
      ```
      public void writeFile() {
		try {
			FileWriter fileWriter = new FileWriter("filename.txt");
			fileWriter.write("Files in Java might be tricky, but it is fun enough!");
			fileWriter.close();
			System.out.println("Successfully wrote to the file.");
		} catch (IOException e) {
			System.out.println("An error occurred.");
			e.printStackTrace();
		}
	}
      ```
  - UI/GUI
    ```
    public void askToUser() {
        Scanner scan = new Scanner(System.in);
        System.out.println("silahkan masukan nama?");
        String nama = scan.nextLine();
        System.out.println("Hello " + nama);
    }
    ```
  - Socket
  
