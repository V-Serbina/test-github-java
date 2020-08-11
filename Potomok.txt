package lera.homeWork21;

public class Potomok {
    private double salary;
    private int workingYears;

public void checkSalary(){
    System.out.println("Salary:"+salary);
    if(workingYears<2){
        salary=salary+(salary*0.05);
    }
    else if (workingYears<=5)
        salary=salary+(salary*0.1);
    else salary=salary+(salary*0.15);
    System.out.println("Increase salary:"+salary);
}





    public double getSalary() {
        return salary;
    }

    public void setSalary(double salary) {
        this.salary = salary;
    }

    public int getWorkingYears() {
        return workingYears;
    }

    public void setWorkingYears(int workingYears) {
        this.workingYears = workingYears;
    }
}
