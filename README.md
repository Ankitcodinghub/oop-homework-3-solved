# oop-homework-3-solved
**TO GET THIS SOLUTION VISIT:** [OOP Homework 3 Solved](https://www.ankitcodinghub.com/product/oop-class-shape-is-fully-implemented-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;112831&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;OOP Homework 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
class Shape

{

STYPE type; public:

Shape();

Shape(STYPE type); virtual void print(); virtual double area();

virtual bool contains(const Shape *s); //Intentionally made non-virtual bool operator==(const Shape &amp;rhs); virtual ~Shape(){}

};

Class Point2D is fully implemented.

class Point2D : public Shape

{

double x,y; public:

Point2D();

Point2D(STYPE argtype, int argx, int argy);

void print(); double area();

bool contains(const Shape * rhs); bool contains(const Point2D * rhs);

bool operator==(const Point2D &amp;rhs);

double getX() const { return x; } double getY() const { return y; }

~Point2D(){}

};

Class Rectangle has some functions which must be implemented.

class Rectangle : public Shape

{

Point2D topRight; Point2D bottomLeft;

Public:

Rectangle();//implement this

Rectangle(STYPE type, Point2D tr, Point2D bl);//implement this void print(); //implement this double area(); //implement this

bool contains(const Shape *rhs); //implement this to check containment for point2d only bool operator==(const Rectangle &amp;rhs); //implement this

~Rectangle(){}

}

Class Circle has some functions which must be implemented.

class Circle : public Shape

{

Point2D center; double radius; public:

Circle();

Circle(STYPE type, Point2D c, double r); //implement this

double area(); //implement this void print(); //implement this bool contains(const Shape * s); //implemented partially bool contains(const Point2D * p); //implement this bool contains(const Circle * rhs); //implement this bool contains(const Rectangle * p); //implement this

bool operator==(const Circle &amp;rhs); //implement this

~Circle(){}

};

Class Point3D has some functions which must be implemented.

class Point3D : public Point2D

{

double z; public:

Point3D(); //already implemented

Point3D(STYPE type, double argx, double argy, double argz); //implement this void print(); //already implemented

//double area(); Not needed, base version is sufficient bool contains(const Shape *rhs); //implement this

bool contains(const Point3D *rhs); //implement this

~Point3D(){}

};

Class Shape3D is fully implemented.

class Shape3D : public Shape

{ public:

Shape3D();

Shape3D(STYPE type); virtual double volume(); ~Shape3D(){}

};

Class Sphere has some functions which must be implemented.

class Sphere : public Shape3D

{

Point3D center; double radius; public:

Sphere();//implement this

Sphere(STYPE type, Point3D c, double r);//implement this void print(); //implement this double area(); //implement this double volume(); //implement this

bool contains(const Shape * rhs); //implement this for checking containgment of Point3D, Sphere inside sphere bool contains(const Point3D * p); //implement this

bool contains(const Sphere * s); //implement this

~Sphere(){}

};
