
#include <Wire.h> 
#include <Adafruit_GFX.h>      //libreria OLED
#include <Adafruit_SSD1306.h>  //libreria OLED 

#define SCREEN_WIDTH 128  //define tamaño de display
#define SCREEN_HEIGHT 64 

Adafruit_SSD1306 display(SCREEN_WIDTH, SCREEN_HEIGHT, &Wire, -1); //

void setup()   
{    

  Serial.begin(9600);  
    display.begin(SSD1306_SWITCHCAPVCC, 0x3C); 
 Serial.println("Inicia programa"); 
//  Clear the buffer.

  // Changing Font Size
  display.clearDisplay();
  display.setTextColor(WHITE);
  display.setCursor(0,24);
  display.setTextSize(3);
  display.println("ACCESA");
  display.display();
  delay(4000);
  display.clearDisplay();
  // Display Text
  display.setTextSize(1);
  display.setTextColor(WHITE);
  display.setCursor(0,10);
   display.setTextSize(2);
  display.println("Introduce tu moneda");
  display.display();
  delay(4000);
 // display.clearDisplay();
  
/////////////////////////// EJEMPLO DE IMPRESION EN RENGLONES///////////////////////////
/*
  display.clearDisplay();
  // Display Text
  display.setTextSize(1);
  display.setTextColor(WHITE);
  display.setCursor(0,10);
  display.println("hola don !");
  display.display();
  delay(4000);
 // display.clearDisplay();
  
    // Display Inverted Text
  display.setTextColor(WHITE); // 'inverted' text
  display.setCursor(0,22);
  display.println("que quiere !");
  display.display();
  delay(4000);
  //display.clearDisplay();
  
  // Display Inverted Text
  display.setTextColor(BLACK, WHITE); // 'inverted' text
  display.setCursor(0,33);
  display.println("comprar elotes ?");
  display.display();
  delay(4000);
  //display.clearDisplay();


*/  
///////////////////////////////////////////////////////////////////////////

/*
  // Display Inverted Text
  display.setTextColor(BLACK, WHITE); // 'inverted' text
  display.setCursor(0,28);
  display.println("que quieres!");
  display.display();
  delay(2000);
  display.clearDisplay();

  // Changing Font Size
  display.setTextColor(WHITE);
  display.setCursor(0,24);
  display.setTextSize(2);
  display.println("Hello!");
  display.display();
  delay(2000);
  display.clearDisplay();

  // Display Numbers
  display.setTextSize(1);
  display.setCursor(0,28);
  display.println(123456789);
  display.display();
  delay(2000);
  display.clearDisplay();

  // Specifying Base For Numbers
  display.setCursor(0,28);
  display.print("0x"); display.print(0xFF, HEX); 
  display.print("(HEX) = ");
  display.print(0xFF, DEC);
  display.println("(DEC)"); 
  display.display();
  delay(2000);
  display.clearDisplay();

  // Display ASCII Characters
  display.setCursor(0,24);
  display.setTextSize(2);
  display.write(3);
  display.display();
  delay(2000);
  display.clearDisplay();
*/

/*
  // Scroll full screen
  display.setCursor(0,0);
  display.setTextSize(1);
  display.println("Full");
  display.println("screen");
  display.println("scrolling!");
  display.display();
  display.startscrollright(0x00, 0x07);
  delay(2000);
  display.stopscroll();
  delay(1000);
  display.startscrollleft(0x00, 0x07);
  delay(2000);
  display.stopscroll();
  delay(1000);    
  display.startscrolldiagright(0x00, 0x07);
  delay(2000);
  display.startscrolldiagleft(0x00, 0x07);
  delay(2000);
  display.stopscroll();
  display.clearDisplay();

  // Scroll part of the screen
  display.setCursor(0,0);
  display.setTextSize(1);
  display.println("Scroll");
  display.println("some part");
  display.println("of the screen.");
  display.display();
  display.startscrollright(0x00, 0x00);
*/
}


void loop() {

}

