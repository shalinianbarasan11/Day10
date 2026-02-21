# 1. How map differs from other collection interface? Explain with an example program

The Map interface in Java is different from List and Set because it does not extend the Collection interface.
A Map stores data in key–value form. Each key is unique. Collections store only values.
A List allows duplicates and index-based access. A Map does not have indexing and uses keys to get values. A Set stores only unique values. A Map also provides keySet(), values() to access keys and values.
Structure:
A Map stores data as key–value pairs.
A List stores elements in an ordered sequence.
A Set stores only unique elements.
Duplicates:
In a Map, keys must be unique, but values can be duplicated.
A List allows duplicate elements.
A Set does not allow duplicate elements.
Access Method:
In a Map, values are accessed using keys with get(key).
In a List, elements are accessed using an index with get(index).
A Set does not support direct index-based access.
### Example
import java.util.ArrayList;
import java.util.HashMap;
import java.util.List;
import java.util.Map;

public class Testcheck{
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		// List example
        List<String> stu = new ArrayList<String>();
        stu.add("Rei");
        stu.add("Anu");
        stu.add("Tanu");  
        System.out.println("Student: " + stu.get(1));  
        
        //Map example
        Map<Integer,String> st = new HashMap<Integer,String>();
        st.put(1, "Tae");
        st.put(2, "Ye jin");
        st.put(3,"Eun bin");  
        
        System.out.println(st); 
		
    }
}
