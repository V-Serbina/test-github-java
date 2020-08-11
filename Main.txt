package lera.homeWork21;


public class Main {
    public static void main(String[] args) {

UserData user1 =  new UserData("newemaili.ua" ,"123");

UserData user2 = new UserData("Valeria","Danilova",77722299,"+308956643289","myemail@i.ua","44557733");
        System.out.println("Password of user1:");
        user1.validPassword();
        System.out.println("Password of user2:");
        user2.validPassword();
        System.out.println("Validation email of user1:");
        if(user1.validEmail()) System.out.println("Ok");
        else System.out.println("NOT OK");
        System.out.println("Validation email of user2:");
        if(user2.validEmail()) System.out.println("Ok");
        else System.out.println("NOT OK");
            System.out.println(user1.getFirstName());
        user1.setSalary(25000);
        user1.setWorkingYears(4);
            System.out.println("Working years:"+user1.getWorkingYears());
        user1.checkSalary();
            System.out.println();

            System.out.println(user2.getFirstName());

            user2.setSalary(44000);
            user2.setWorkingYears(6);
            System.out.println("Working years:"+user2.getWorkingYears());
            user2.checkSalary();


    }
}
