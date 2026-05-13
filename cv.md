# Hello! I'm Shekolyan N.D.

 

- [About myself](#About)
- [Skills](#Skills)
- [Code example](#Code)
- [Projects](#Projects)
- [Contacts](#Contacts)
- [Languages](#Languages)
- [Picture](#Picture)

 

## About myself

 

I'm a beginner IT specialist. I have experience working with Python and am currently learning HTML and C#.

 

## Skills

 

1. Python
2. C#
3. HTML

 

## Code example

 

```

                import math

                def f(x):
                return 0.5 * (x) - math.log10(x + 1) - 0.5

                def root_separation(a, b, h):
                intervals = []
                x = a
                while x < b:
                if f(x) * f(x+h) < 0:
                intervals.append((x, x + h))
                x = x + h
                return intervals

                def half_div(a, b, eps):
                while (b - a) > eps:
                c = (a + b) / 2
                if f(a) * f(c) < 0:
                b = c
                else:
                a = c
                return (a + b) / 2

                a = float(input("Введите левую границу: "))
                b = float(input("Введите правую границу: "))
                eps = float(input("Введите точность: "))
                h = float(input("Введите шаг: "))

                intervals = root_separation(a, b, h)

                n = 1
                for interval in intervals:
                print()
                print(f"{n}-й корень уравнения")
                root = half_div(interval[0], interval[1], eps)
                print(root)
                n += 1
            
```
