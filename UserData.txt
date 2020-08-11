package lera.homeWork21;

public class UserData extends Potomok{

    private String firstName;
    private String secondName;
    private double workPhone;
    private  String mobilePhone;
    private String email;
    private  String password;

    public UserData(String firstName, String secondName, double workPhone, String mobilePhone, String email, String password) {
        this.firstName = firstName;
        this.secondName = secondName;
        this.workPhone = workPhone;
        this.mobilePhone = mobilePhone;
        this.email = email;
        this.password = password;
    }

    public UserData(String email, String password) {
        this.email = email;
        this.password = password;
    }
public void validPassword(){
        if(16<password.length()||password.length()<4)
            System.out.println("Wrong lenght. Must be more then 4 and less then 16");
        else System.out.println("Ok");
}

public boolean validEmail(){
        String em = email;
        boolean h = false;
    for (int i = 0; i < email.length(); i++) {
        char q = em.charAt(i);
        if(q=='@'){
            h= true;}

    }
    if(h==true)return true;
    else return false;

}




    public String getFirstName() {
        return firstName;
    }

    public void setFirstName(String firstName) {
        this.firstName = firstName;
    }

    public String getSecondName() {
        return secondName;
    }

    public void setSecondName(String secondName) {
        this.secondName = secondName;
    }

    public double getWorkPhone() {
        return workPhone;
    }

    public void setWorkPhone(double workPhone) {
        this.workPhone = workPhone;
    }

    public String getMobilePhone() {
        return mobilePhone;
    }

    public void setMobilePhone(String mobilePhone) {
        this.mobilePhone = mobilePhone;
    }

    public String getEmail() {
        return email;
    }

    public void setEmail(String email) {
        this.email = email;
    }

    public String getPassword() {
        return password;
    }

    public void setPassword(String password) {
        this.password = password;
    }
}
