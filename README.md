     if (args[0].equals("l")) {
            System.out.println("Loading data ...");
            try {
                BufferedReader r = new BufferedReader(
                        new InputStreamReader(
                                new FileInputStream("employees.txt")));
                BufferedReader r = new BufferedReader(new InputStreamReader(new FileInputStream("employees.txt")));
                String l = r.readLine();
                String e[] = l.split(",");
                for (String emp : e) {
                    System.out.println(emp);
                }
            } catch (Exception e) {}
            } 
            catch (Exception e) {}
            System.out.println("Data Loaded.");
        } else if (args[0].equals("s")) {
        } 
        else if (args[0].equals("s")) {
            System.out.println("Loading data ...");

            try {
                BufferedReader r = new BufferedReader(
                        new InputStreamReader(
                                new FileInputStream("employees.txt")));
                BufferedReader r = new BufferedReader(new InputStreamReader(new FileInputStream("employees.txt")));
                String l = r.readLine();
                System.out.println(l);
                String e[] = l.split(",");
                Random rand = new Random();
                int idx = rand.nextInt(e.length);
                System.out.println(e[idx]);
            } catch (Exception e) {}
            }catch (Exception e) {}

            System.out.println("Data Loaded.");
        } else if (args[0].contains("+")) {
        } 
        else if (args[0].contains("+")) {
            System.out.println("Loading data ...");
            try {
                BufferedWriter w = new BufferedWriter(
                        new FileWriter("employees.txt", true));
                String n = args[0].substring(1);
                w.write(", " + n);
                w.close();
            } catch (Exception e) {}
            } 
            catch (Exception e) {}

            System.out.println("Data Loaded.");
        } else if (args[0].contains("?")) {
        } 
        else if (args[0].contains("?")) {
            System.out.println("Loading data ...");
            try {
                BufferedReader r = new BufferedReader(
                        new InputStreamReader(
                                new FileInputStream("employees.txt")));
                BufferedReader r = new BufferedReader(new InputStreamReader(new FileInputStream("employees.txt")));
                String l = r.readLine();
                String e[] = l.split(",");
                boolean found = false;
@@ -58,14 +60,14 @@ public static void main(String[] args) {
                        found = true;
                    }
                }
            } catch (Exception e) {}
            } 
            catch (Exception e) {}
            System.out.println("Data Loaded.");
        } else if (args[0].contains("c")) {
        } 
        else if (args[0].contains("c")) {
            System.out.println("Loading data ...");
            try {
                BufferedReader r = new BufferedReader(
                        new InputStreamReader(
                                new FileInputStream("employees.txt")));
                BufferedReader r = new BufferedReader(new InputStreamReader(new FileInputStream("employees.txt")));
                String l = r.readLine();
                char[] chars = l.toCharArray();
                boolean inWord = false;
@@ -81,14 +83,14 @@ public static void main(String[] args) {
                    }
                }
                System.out.println(count + " word(s) found " + chars.length);
            } catch (Exception e) {}
            } 
            catch (Exception e) {}
            System.out.println("Data Loaded.");
        } else if (args[0].contains("u")) {
        } 
        else if (args[0].contains("u")) {
            System.out.println("Loading data ...");
            try {
                BufferedReader r = new BufferedReader(
                        new InputStreamReader(
                                new FileInputStream("employees.txt")));
                BufferedReader r = new BufferedReader(new InputStreamReader(new FileInputStream("employees.txt")));
                String l = r.readLine();
                String e[] = l.split(",");
                String n = args[0].substring(1);
@@ -101,9 +103,11 @@ public static void main(String[] args) {
                        new FileWriter("employees.txt"));
                w.write(String.join(",", e));
                w.close();
            } catch (Exception e) {}
            } 
            catch (Exception e) {}
            System.out.println("Data Updated.");
        } else if (args[0].contains("d")) {
        } 
        else if (args[0].contains("d")) {
            System.out.println("Loading data ...");
            try {
                BufferedReader r = new BufferedReader(
