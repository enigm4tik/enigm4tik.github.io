## Learning C++

Yesterday I've mentioned that I'm now learning C++ "properly", now, how do I do that?  
During my studies (in university) my professor suggested watching videos by The Cherno on Game Engine Design and then learn from there. 
In fact, instead of teaching us these principles in class, we were assigned to watch the videos at home and then answer some questions in class.  
Since I didn't really like this approach of teaching, I didn't appreciate the amount of work and the straight-forwardness of his videos.

Now, studying on my own, I'm now going over the 101 videos in [The Cherno's C++ playlist](https://www.youtube.com/playlist?list=PLlrATfBNZ98dudnM48yfGUldqGD0S4FFb) and try to understand as much as I can. 
Writing code and notes while watching and looking up things I don't fully understand, I am really grateful such a comprehensive resource exists.
I'm currently at video 40 and today I've learned about `implicit vs. explicit conversion`, `the new keyword` and `operators and overloading them`.

_______

### Day 2

So, for day 2, here's a struct of a Vector2 and a simple overloaded operator.

```cpp
struct Vector2
{
	float x, y;

	Vector2(float x, float y)
		: x(x), y(y) {}

	Vector2 operator+(const Vector2& other)
	{
		return Vector2 (x + other.x, y + other.y);
	}
};

int main()
{
	Vector2 a(0.0f, 0.0f);
	Vector2 b(1.1f, 1.2f);

	Vector2 result = a + b;

	return 0;
}
```

See you tomorrow!

```cpp
string greeting = "enigm4tik";
``` 