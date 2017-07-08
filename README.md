# Java-Concepts

<ul>
<li><a href="#Creating-Generic-Classes-In-Java">Creating Generic Classes In Java</a></li>
<li><a href="#Creating-Generic-Classes-with-multiple-types">Creating Generic Classes with multiple types</a></li>
<li><a href="#Creating-generic-method-inside-non-generic-class">Creating generic method inside non generic class</a></li>
</ul>



<a name="#Creating-Generic-Classes-In-Java"><b>Creating Generic Classes In Java</b></a>
<hr>

```
public class GList<T>
{
	private T[] myList;
	private int size;
	private int position;
	public GList(int s)
	{
		myList = (T[])new Object[size];
		this.size=s;
		this.position = 0;
	}

}
```

<br/>


<a name="Creating-Generic-Classes-with-multiple-types"><b>Creating Generic Classes with multiple types</b></a>
<hr>

```

public class Pair<T,U>
{
	private T first;
	private U second;
	public Pair(T first,U second)
	{	
		this.first= first;
		this.second= second;
	}
	
	public T first()
	{
		return first;
	}
	public U second()
	{
		return second;
	}
}

```

<br/>

<a name="Creating-generic-method-inside-non-generic-class"><b>Creating generic method inside non generic class</b></a>

<hr>

```
class GenericMethod
{
	static <T> void Display(T[] arr)
	{	
		for(int i=0;i<arr.length;i++)
		{
			if(arr[i]!=null) System.out.print(arr[i]+" ");
		}
	}

	public static void main(String args[])
	{
		Integer ar[] = new Integer[]{0,1,2,3,4,5};
		Display(ar);
	}
}

```
