using System;

class AreaCalculator
{
    // Method to calculate the area of a circle
    static double CircleArea(double radius)
    {
        return 3.14 * radius * radius;
    }
    static double TriangleArea(double baseLength, double height)
    {
        return 0.5 * baseLength * height;
    }
 static double RectangleArea(double length, double width)
    {
        return length * width;
    }

 calculate the area of a regular pentagon
    static double PentagonArea(double side)
    {
        return (5 * side * side) / (4 * Math.Tan(Math.PI / 5));
    }
    static double OctagonArea(double side)
    {
        return 2 * (1 + Math.Sqrt(2)) * side * side;
    }

    static void Main()
    {
        Console.WriteLine("Area of Circle (r=5): " + CircleArea(5));
        Console.WriteLine("Area of Triangle (b=10, h=6): " + TriangleArea(10, 6));
        Console.WriteLine("Area of Rectangle (l=8, w=4): " + RectangleArea(8, 4));
        Console.WriteLine("Area of Pentagon (s=7): " + PentagonArea(7));
        Console.WriteLine("Area of Octagon (s=6): " + OctagonArea(6));
    }
}
