# CubeCalculator
Coded in Java

      import java.lang.Math; 

      class Main {

        //assign varriables
      static double sideLength = 1;
      static double AreaOfOneFace = 0;
      static double AreaOfSixFaces = 0;
      static double VolOfCube = 0;

      public static void main(String[] args) {
      //call functions
      AreaOfOneFace = calcAreaOfOneFace();
      AreaOfSixFaces = calcAreaOfSixFaces();
      VolOfCube = calcVolOfCube();

      //print
      System.out.println("Method 1: calcAreaOfOneFace() - the output of this function will be");
      System.out.println("Given a side of length " + sideLength + ", the area of one face is " + AreaOfOneFace);
      System.out.println();

      System.out.println("Method 2: calcAreaOfSixFaces() - the output of this function will be");
      System.out.println("Given a side of length " + sideLength + ", of area of the sums of all the faces is " + AreaOfSixFaces);
      System.out.println();

      System.out.println("Method 3: calcVolOfCube() - the output of this function will be");
      System.out.println("Given a side of length " + sideLength + "  of volume of the cube is " + VolOfCube);
      System.out.println();
    }

    public static double calcAreaOfOneFace() {
      //Method 1: calcAreaOfOneFace()  -   the output of this function will be 
      //"Given a side of length 1, the area of one face is 1."   
      return (sideLength*sideLength);
    }

    public static double calcAreaOfSixFaces() {
      //Method 2: calcAreaOfSixFaces() - the output of this function will be
      //"Given a side of length 1,  of area of the sums of all the faces is 6."
      return (6*AreaOfOneFace);
    }

    public static double calcVolOfCube() {
      //Method 3: calcVolOfCube() - the output of this function will be
      //"Given a side of length 1,  of volume of the cube is 1."
      return Math.pow(sideLength, 3);
    }
    }
