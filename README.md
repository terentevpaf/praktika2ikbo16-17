# praktika2ikbo16-17
# Терентьев Павел


# Класс Author
<pre>
public class Author {
    private String name;
    private String email;
    private char gender;
    Author(String name, String email, char gender){
        this.name = name;
        this.email = email;
        if(gender == 'M')
        {
            gender = 'M';
        }
        else if(gender == 'F') {
            gender = 'F';
        }
        else {
            gender = 'U';
        }
        this.gender = gender;
    }
    public void setEmail(String email) {
        this.email = email;
    }
    public String getName() {
        return name;
    }
    public String getEmail() {
        return email;
    }
    public char getGender() {
        return gender;
    }
    @Override
    public String toString() {
        return "Author: " + getName() + " (" + getGender() + "), " + getEmail();
    }
}

</pre>

# Класс TestAuthor
<pre>
import java.lang.*;
public class TestAuthor {
    public static void main(String[] args) {
        Author at = new Author("Pavel-1", "pavel-1@mail.ru", 'A');
        System.out.println(at.toString());
        at = new Author("Pavel-2", "pavel-2@mail.ru", 'F');
        System.out.println(at.toString());
    }
}
</pre>
