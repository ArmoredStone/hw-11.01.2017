package com.company;

import java.io.*;
import java.nio.Buffer;

public class Reader {
    public static void file(File file, int number) {
        String content = "";
           try {
            FileReader fr = new FileReader(file);
            BufferedReader br = new BufferedReader(fr);
            String buffer;
            while ((buffer = br.readLine()) != null) {
                content += buffer;
            }
        } catch (FileNotFoundException e) {
            e.printStackTrace();
        } catch (IOException e) {
            e.printStackTrace();
        }
    String[] done = content.split(" ");
           if (number>done.length){
               System.out.println("Извините, в данном файле не так много слов :с");
               System.exit(0);
           }
        System.out.print("Слово под номером "+number+" - "+done[number-1]);
    }

}
