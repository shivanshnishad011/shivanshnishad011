
// Define the Playable interface
interface Playable {
    void play();
}

// Guitar class implements Playable
class Guitar implements Playable {
    @Override
    public void play() {
        System.out.println("Strumming the guitar!");
    }
}

// Piano class implements Playable
class Piano implements Playable {
    @Override
    public void play() {
        System.out.println("Playing the piano!");
    }
}

// Main class to demonstrate polymorphism
public class MusicDemo {
    public static void main(String[] args) {
        Playable instrument1 = new Guitar();  // Upcasting
        Playable instrument2 = new Piano();   // Upcasting

        instrument1.play();  // Will call Guitar's play()
        instrument2.play();  // Will call Piano's play()
    }
}
