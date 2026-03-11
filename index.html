import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

import java.io.FileOutputStream;
import java.io.InputStream;
import java.net.URL;
import java.util.List;

public class PexelsScraper {

    public static void main(String[] args) throws Exception {

        System.setProperty("webdriver.chrome.driver","C:/chromedriver/chromedriver.exe");

        WebDriver driver = new ChromeDriver();

        // search page
        driver.get("https://www.pexels.com/search/nature/");

        Thread.sleep(5000); // wait for images

        List<WebElement> images = driver.findElements(By.tagName("img"));

        int count = 0;

        for(WebElement img : images){

            try{

                String src = img.getAttribute("src");

                if(src == null) continue;

                if(!src.startsWith("https")) continue;

                URL url = new URL(src);
                InputStream in = url.openStream();

                FileOutputStream out = new FileOutputStream("pexels_image_"+count+".jpg");

                byte[] buffer = new byte[2048];
                int length;

                while((length = in.read(buffer)) != -1){
                    out.write(buffer,0,length);
                }

                in.close();
                out.close();

                System.out.println("Downloaded: " + src);

                count++;

            }catch(Exception e){
                System.out.println("Skipped");
            }

            if(count >= 5) break;
        }

        driver.quit();
    }
}
