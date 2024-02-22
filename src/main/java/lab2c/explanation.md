Yau Wai Keung
20854940

# Part1
Yau Wai Keung
20854940


package lab2b;

public class Book {
private String chapters[];
private static final int DEFAUT_CHATERS = 10;

    public Book(){
        chapters = new String[DEFAUT_CHATERS];
        for(int i = 0; i < chapters.length; i++)
            chapters[i] = "n/a";
    }

    public Book(String argument[]){
        chapters = new String[argument.length];
        for(int i = 0; i < argument.length; i++)
            chapters[i] = argument[i];
    }

    public String getChapter(int i){
        return chapters[i];
    }

    public String[] getChapters(){
        return chapters;
    }
}

# Part2

package lab2c;

public class MobileComputer extends Computer implements Chargeable{
private int battery;
public MobileComputer(){
secret = "MobileComputer secret";
battery = 5;
}

    @Override
    public void work() {
        if(battery > 0){
            System.out.println("It is working on my lap.");
            battery--;
        }
        else{
            System.out.println("Running out of battery");
        }
    }
    public void charge(){
        if(battery < 10){
            battery ++;
        }
    }
}

## explanation
To use the interface of Charger, we need to implement the interface of Charger in MobileComputer. 
