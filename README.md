# Java-Concepts

<b>Creating Generic Classes In Java</b>
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


<b>Creating Generic Classes with multiple types</b>
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
<b>Creating generic method inside non generic class</b>
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
