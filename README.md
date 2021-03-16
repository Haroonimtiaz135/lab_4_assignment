# lab_4_assignment

public class HotDogStand {
    private int id_number;
    private int no_of_hot_dogs;
    
    public HotDogStand(int x, int y){
        id_number = x;
        no_of_hot_dogs = y;
    
    }
    
    public int getidnum(){
        return id_number;
    }
    
    
    public void justsold(int z){
        no_of_hot_dogs = no_of_hot_dogs + z;
        
        
    }
    
    public int gethotdogs(){
      return no_of_hot_dogs;
    }
    
    
    
    
}


package hotdogstand;

public class hotdogstand_runner {
    public static void main(String[]args){
        HotDogStand h1 = new HotDogStand(324156, 7);
        h1.justsold(3);
        h1.justsold(7);
        System.out.println("the total number of hotdogs sold by id number :"+h1.getidnum()+" is : "+h1.gethotdogs());
        
        HotDogStand h2 = new HotDogStand(324157, 2);
        h2.justsold(9);
        System.out.println("the total number of hotdogs sold by id number :"+h2.getidnum()+" is : "+h2.gethotdogs());
        
        HotDogStand h3 = new HotDogStand(324198, 12);
        h3.justsold(1);
        System.out.println("the total number of hotdogs sold by id number :"+h3.getidnum()+" is : "+h3.gethotdogs());
        
        
    }
}
