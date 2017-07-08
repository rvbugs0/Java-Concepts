# Java-Concepts

<b>Creating Generic Classes In Java</b>
<hr>

<code>
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
</code>