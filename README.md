# RandomPhraseGenerator
RandomPhraseGenerator
import java.util.Random;

public class RandomPhraseGenerator {
    public static void main(String[] args) {
        String[] nouns = { "кошка", "автомобиль", "дом", "солнце", "книга" };
        String[] verbs = { "бежит", "прыгает", "поет", "играет", "спит" };
        String[] adjectives = { "красивый", "быстрый", "веселый", "интересный", "успешный" };

        Random random = new Random();

        String noun = nouns[random.nextInt(nouns.length)];
        String verb = verbs[random.nextInt(verbs.length)];
        String adjective = adjectives[random.nextInt(adjectives.length)];

        String phrase = "Я " + adjective + " " + noun + " " + verb + "!";
        System.out.println(phrase);
    }
}
