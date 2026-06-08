### Question -  Find Shortest Path 
1) Given a route containing 4 directions ( E , W, N , S). Find the shortest path to reach destination?
"WNEENESENNN"

   ``` Java - Code

    import java.util.*;
   class file {
   public static float findShortestPath(String path){
     int x = 0, y =0; // initialized x and y with zero
   
     for( int i=0; i< path.length(); i++){
    
       char dir = path.charAt(i); //making a variable which store direction   

   if( dir == 'S'){
      y--;
   }
    else if( dir == 'N'){

        y++;
   }

   else if(dir == 'W'){

     x--;
   
   }
   else{
     x++;
   }
   
   }

      int X2 = x*x;
      int Y2 = y*y;
   return (float)Math.sqrt(X2 + Y2);
   }
   public static void main(String args[]){

         String  path = "WNEENESENNN";
          System.out.println(findShortestPath(path));
   }

   }
   ```




   ## Input - WNEENESENNN

   ## Output - 5.0
   
