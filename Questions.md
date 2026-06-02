## تحليل المحتوى (Analysis Summary)

تم تحليل ملفات المحاضرات الأربعة (Computer Graphics) والتي تغطي الموضوعات التالية:

**الملف الأول (Lecture 1): Graphics Systems**
- تعريف رسومات الحاسوب ومجالات التطبيق (التصميم، المحاكاة، الواقع الافتراضي، معالجة الصور، الواجهات).
- مكونات نظام الرسومات: CPU، GPU، Frame Buffer، أجهزة الإدخال والإخراج.
- مفهوم البكسل (Pixel) وذاكرة الإطار (Frame Buffer) من حيث الحجم (Resolution) والعمق (Depth) مثل 1-bit، 8-bit، 24-bit.
- شرح شاشات CRT وآلية عملها، ودقة الشاشة (VGA, SVGA, WXGA) ونسبة الأبعاد.
- الفرق بين الصور النقطية (Raster) والمتجهية (Vector) وأمثلة على صيغ الملفات (JPEG, PNG, AI, CDR).
- مفهوم التصيير (Rendering) والتحويل من 3D إلى 2D.

**الملف الثاني (Lecture 2): Graphics Primitives & HTML5 Canvas**
- الأوليات الهندسية (Primitives) ثنائية وثلاثية الأبعاد وسماتها (اللون، السمك، الموضع).
- أساسيات الهندسة: الكميات القياسية (Scalars) والمتجهات (Vectors) والنقاط (Points).
- عمليات المتجهات: الطول (Magnitude) والضرب النقطي (Dot Product) والعلاقة بالزاوية بين المتجهات.
- أنظمة الإحداثيات (Cartesian) والمواقع المطلقة مقابل النسبية (Absolute vs Relative).
- خوارزميات رسم الخط المستقيم (DDA) والدائرة (باستخدام المعادلة `x^2 + y^2 = r^2` والطريقة القطبية).
- مقدمة إلى JavaScript وكيفية تضمينها في HTML.
- عنصر Canvas في HTML5: رسم المسارات (paths)، المستطيلات، الأقواس (arcs)، والدوائر مع أمثلة كود.

**الملف الثالث (Lecture 3): Transformations**
- التحويلات الهندسية: الإزاحة (Translation) والقياس (Scaling) والتدوير (Rotation) والقص (Shear) والانعكاس (Reflection).
- استخدام الإحداثيات المتجانسة (Homogeneous Coordinates) لتمثيل التحويلات بمصفوفات 3×3 للـ 2D و4×4 للـ 3D.
- مصفوفات التحويل لكل عملية (Translation, Rotation, Scaling, Shear, Reflection).
- التحويل حول نقطة اعتباطية (Rotation about arbitrary point) من خلال الإزاحة ثم التدوير ثم الإزاحة العكسية.
- أمثلة محلولة: تكبير مثلث، إزاحة مستطيل، تدوير مستطيل حول مركزه.
- التحويلات ثلاثية الأبعاد: التدوير حول المحاور X, Y, Z.
- تطبيقات التحويلات في HTML5 Canvas باستخدام `scale()`, `rotate()`, `transform()`.

**الملف الرابع (Lecture 4): Colors**
- فيزياء اللون وعلاقته بالضوء والجسم والمراقب.
- الألوان الأولية (Primary: R,G,B) والثانوية (Secondary: C,M,Y) وأطوالها الموجية.
- نماذج الألوان: RGB (للشاشات)، CMYK (للطابعات)، HSV (Hue, Saturation, Value)، YIQ (للتلفزيون التناظري).
- الفرق بين الألوان الجمعية (Additive - RGB) والطرحّية (Subtractive - CMYK).
- التحويل بين نماذج RGB وCMYK و YIQ.
- تمثيل الألوان في HTML5: السلاسل النصية (`'red'`)، النظام الست عشري (`#ff0000`)، RGB (`rgb(255,0,0)`).
- التدرجات اللونية: الخطية (Linear Gradient) والشعاعية (Radial Gradient) مع أمثلة أكواد.

---

# بنك الأسئلة (MCQ Bank) - 90 سؤالاً

## القسم الأول: أنظمة الرسومات الأساسية (Graphics Systems Basics) - الأسئلة 1-15

**س1:** Which of the following best defines computer graphics?
A) The study of algorithms for sorting graphical data
B) The study of creating, manipulating, and using visual images in a computer
C) The process of printing images using a laser printer
D) The hardware components of a computer only

**الإجابة الصحيحة: B**

**س2:** Which component is specifically designed to perform complex mathematical calculations necessary for graphics rendering?
A) CPU
B) GPU
C) RAM
D) Frame Buffer

**الإجابة الصحيحة: B**

**س3:** The memory that holds pixel properties such as color and depth is called:
A) Cache memory
B) Virtual memory
C) Frame buffer
D) Hard disk buffer

**الإجابة الصحيحة: C**

**س4:** If a frame buffer has 24 bits per pixel, how many colors can it display?
A) 256 colors
B) 65,536 colors
C) 16,777,216 colors
D) 16 colors

**الإجابة الصحيحة: C**

**س5:** Which screen resolution corresponds to WXGA?
A) 640 x 480
B) 800 x 600
C) 1366 x 768
D) 1920 x 1080

**الإجابة الصحيحة: C**

**س6:** What is the function of the electron gun in a CRT monitor?
A) To store pixel data
B) To emit a beam of electrons to the phosphorescent screen
C) To compute geometric transformations
D) To process keyboard input

**الإجابة الصحيحة: B**

**س7:** Which of the following is an example of a vector image format?
A) .jpg
B) .png
C) .gif
D) .ai

**الإجابة الصحيحة: D**

**س8:** The process of breaking an image into a grid of pixels is called:
A) Vectorization
B) Rasterization
C) Transformation
D) Clipping

**الإجابة الصحيحة: B**

**س9:** Which of the following is NOT a major application area of computer graphics mentioned in the lecture?
A) Display of information
B) Design
C) Database management
D) Simulation and animation

**الإجابة الصحيحة: C**

**س10:** In a frame buffer with 1 bit per pixel, what is the maximum number of colors that can be produced?
A) 1 color
B) 2 colors (typically black and white)
C) 256 colors
D) 16 million colors

**الإجابة الصحيحة: B**

**س11:** Which device is associated with Ivan Sutherland's Sketchpad and light-pen?
A) Virtual Reality headset
B) User interface for computer graphics
C) Color printer
D) Digital camera

**الإجابة الصحيحة: B**

**س12:** What does "depth" refer to in the context of a frame buffer?
A) The physical size of the monitor
B) The number of bits used per pixel (color level)
C) The 3D effect of the image
D) The refresh speed of the monitor

**الإجابة الصحيحة: B**

**س13:** Which of the following statements about GPU is FALSE?
A) GPU is similar to a computer's CPU but specialized for graphics
B) GPU is responsible for rasterizing pictures into pixels
C) Recent GPUs contain over 100 processing units
D) GPUs cannot be used for general purpose computing

**الإجابة الصحيحة: D**

**س14:** What is the aspect ratio of a screen with width 1024 pixels and height 768 pixels?
A) 1.33:1
B) 4:3
C) Both A and B
D) 16:9

**الإجابة الصحيحة: C** (4:3 = 1.33:1)

**س15:** Which image type records images descriptively using mathematics to identify lines and geometric shapes?
A) Raster image
B) Bitmap image
C) Vector image
D) Pixel image

**الإجابة الصحيحة: C**

---

## القسم الثاني: تطبيقات رسومات الحاسوب (Applications) - الأسئلة 16-25

**س16:** Which application area includes flight simulators, driving simulators, and surgical simulation?
A) Computer-Aided Design
B) Scientific Visualization
C) Visual Simulation and Training
D) Digital Media Technologies

**الإجابة الصحيحة: C**

**س17:** Which software is mentioned as an example of Computer-Aided Design (CAD)?
A) Adobe Photoshop
B) Sketchup
C) Microsoft Word
D) VLC Media Player

**الإجابة الصحيحة: B**

**س18:** What is the purpose of 2D Rendering?
A) To convert a 2D image into a 3D model
B) To create a 2D image from a 3D model
C) To edit image colors only
D) To print images directly

**الإجابة الصحيحة: B**

**س19:** Which of the following is an example of Digital Media Technology?
A) Apollo spacecraft
B) Surgical simulation
C) Inkjet and laser printers
D) The Virtual Human Karl-Heinz Hoehne

**الإجابة الصحيحة: C**

**س20:** In animation, what is used to represent motion?
A) Only keyframes
B) Sequence of images and parameter curves
C) Only text descriptions
D) Audio files only

**الإجابة الصحيحة: B**

**س21:** Which application uses immersive interfaces with input devices like 3D 6-DOF tracking and gloves?
A) User Interfaces
B) Virtual Reality
C) Image Editing
D) Scientific Visualization

**الإجابة الصحيحة: B**

**س22:** The process of moving or simulating the movement of an object over time is called:
A) Rendering
B) Modeling
C) Animation
D) Rasterization

**الإجابة الصحيحة: C**

**س23:** Which of the following is NOT a typical application of computer graphics?
A) Digital photography
B) Electronic books
C) Audio compression
D) Graphics on the web

**الإجابة الصحيحة: C**

**س24:** What does "Motion blur" in computer graphics refer to?
A) Blurring the background intentionally
B) The effect of fast-moving objects appearing blurred
C) A type of image filter for still images
D) A color model

**الإجابة الصحيحة: B**

**س25:** The composition of real and virtual scenes is known as:
A) Augmented Reality (implied)
B) Vector graphics
C) Raster graphics
D) Image cropping

**الإجابة الصحيحة: A** (يستنتج من المحتوى)

---

## القسم الثالث: الأوليات الهندسية والمتجهات (Primitives & Vectors) - الأسئلة 26-40

**س26:** Which of the following is a 2D geometric primitive?
A) Sphere
B) Polyhedron
C) Circle
D) Light source

**الإجابة الصحيحة: C**

**س27:** Which of the following is a primitive attribute?
A) Color
B) Thickness
C) Position
D) All of the above

**الإجابة الصحيحة: D**

**س28:** In geometry, what does a point represent?
A) A direction in space
B) A location in space
C) A displacement between two positions
D) A scalar quantity

**الإجابة الصحيحة: B**

**س29:** What does a vector represent?
A) A location in space
B) A scalar quantity only
C) A displacement between points or a direction
D) The color of a pixel

**الإجابة الصحيحة: C**

**س30:** What is the result of subtracting one point from another point?
A) Another point
B) A vector
C) A scalar
D) A color

**الإجابة الصحيحة: B**

**س31:** The formula `U · V = ||U|| * ||V|| * cos(angle(U,V))` defines:
A) Cross product
B) Dot product
C) Vector addition
D) Scalar multiplication

**الإجابة الصحيحة: B**

**س32:** If the dot product of two non-zero vectors is zero, what can be concluded?
A) The vectors are parallel
B) The vectors are orthogonal (perpendicular)
C) The vectors are identical
D) The vectors have equal magnitude

**الإجابة الصحيحة: B**

**س33:** The magnitude (length) of a vector V = (6, -15, 10) is:
A) 19
B) 31
C) 361
D) 10

**الإجابة الصحيحة: A** (√(36+225+100) = √361 = 19)

**س34:** Which operation on vectors yields a scalar result?
A) Cross product
B) Dot product
C) Vector subtraction
D) Vector addition

**الإجابة الصحيحة: B**

**س35:** In 2D Cartesian coordinates, which coordinate pair represents a point?
A) [x, y]
B) [x, y, z]
C) [magnitude, direction]
D) [r, θ]

**الإجابة الصحيحة: A**

**س36:** Relative positioning in graphics is related to which linear algebra concept?
A) Point
B) Scalar
C) Vector (displacement)
D) Matrix

**الإجابة الصحيحة: C**

**س37:** Which of the following is NOT a fundamental operator on vectors mentioned in the lecture?
A) Dot product
B) Cross product
C) Mixed product (triple product)
D) Division product

**الإجابة الصحيحة: D**

**س38:** A scalar in geometry:
A) Has both magnitude and direction
B) Alone has no geometric properties
C) Represents a location in space
D) Always represents a color

**الإجابة الصحيحة: B**

**س39:** If the dot product of two vectors is negative, the angle between them is:
A) 0°
B) Acute (less than 90°)
C) 90°
D) Obtuse (greater than 90°)

**الإجابة الصحيحة: D**

**س40:** What is the zero vector?
A) A vector with zero magnitude and undefined orientation
B) A point at the origin
C) A scalar with value zero
D) A vector perpendicular to all other vectors

**الإجابة الصحيحة: A**

---

## القسم الرابع: خوارزميات الرسم (Drawing Algorithms) - الأسئلة 41-50

**س41:** The DDA (Digital Difference Analyzer) algorithm is used for:
A) Drawing circles
B) Drawing lines
C) Filling polygons
D) Anti-aliasing

**الإجابة الصحيحة: B**

**س42:** In the DDA algorithm, if the slope m = 3/5, starting from (0,1) to (5,4), how is y calculated for each x increment?
A) y = y + 1
B) y = y + 3/5
C) y = y * 3/5
D) y = y - 3/5

**الإجابة الصحيحة: B** (Yi+1 = yi + m)

**س43:** Which of the following is a special case for line conversion where both x and y coordinates are incremented by 1?
A) Horizontal line
B) Vertical line
C) Diagonal line (slope = 1)
D) Arbitrary line

**الإجابة الصحيحة: C**

**س44:** The simple circle drawing algorithm using `y = ±√(r² - x²)` suffers from which problem?
A) It only draws circles in color
B) It is inefficient due to square root calculations and uneven spacing
C) It cannot draw filled circles
D) It only works for small radii

**الإجابة الصحيحة: B**

**س45:** The polar method for circle drawing uses which parametric equations?
A) x = r * sinθ, y = r * cosθ
B) x = xc + r * cosθ, y = yc + r * sinθ
C) x = xc + r * θ, y = yc + r * θ
D) x = r * tanθ, y = r * cotθ

**الإجابة الصحيحة: B**

**س46:** To draw a circle using the polar method, the range of θ is typically:
A) 0 to π
B) 0 to 2π
C) 0 to π/2
D) -π to π

**الإجابة الصحيحة: B**

**س47:** In the context of line drawing, what does "round(y)" in the DDA algorithm signify?
A) The integer part of y
B) The nearest integer to y
C) The floor of y
D) The ceiling of y

**الإجابة الصحيحة: B**

**س48:** What defines an arc in computer graphics?
A) Only a radius
B) A center point, radius, start angle, end angle, and direction
C) Two endpoints only
D) A center point and chord length

**الإجابة الصحيحة: B**

**س49:** The slope of a line between points (x1,y1) and (x2,y2) is calculated as:
A) (x2 - x1) / (y2 - y1)
B) (y2 - y1) / (x2 - x1)
C) (y2 + y1) / (x2 + x1)
D) Δx / Δy

**الإجابة الصحيحة: B**

**س50:** For a vertical line, the DDA algorithm would:
A) Increment x by 1 and keep y constant
B) Increment y by 1 and keep x constant
C) Increment both x and y by 1
D) Throw an error because slope is infinite

**الإجابة الصحيحة: B** (منطقياً، لكن السؤال يقيس فهم الحالات الخاصة)

---

## القسم الخامس: HTML5 Canvas وجافا سكريبت (JavaScript & Canvas) - الأسئلة 51-58

**س51:** How do you obtain a 2D rendering context from a canvas element?
A) canvas.getContext("2d")
B) canvas.getContext("3d")
C) canvas.getRenderingContext()
D) canvas.get2D()

**الإجابة الصحيحة: A**

**س52:** Which method begins a new path in HTML5 Canvas?
A) startPath()
B) newPath()
C) beginPath()
D) initPath()

**الإجابة الصحيحة: C**

**س53:** To draw a rectangle with only an outline (no fill) in Canvas, you would use:
A) fillRect()
B) drawRect()
C) strokeRect()
D) rect() only

**الإجابة الصحيحة: C**

**س54:** Which JavaScript method is used to draw an arc (or circle) on a canvas?
A) drawArc()
B) circle()
C) arc()
D) curve()

**الإجابة الصحيحة: C**

**س55:** What is the correct way to set the fill color to yellow in Canvas?
A) context.fill = "yellow"
B) context.fillStyle = "yellow"
C) context.color = "yellow"
D) context.setColor("yellow")

**الإجابة الصحيحة: B**

**س56:** Which HTML tag is used to embed JavaScript code externally?
A) `<script src="file.js">`
B) `<link src="file.js">`
C) `<javascript src="file.js">`
D) `<js file="file.js">`

**الإجابة الصحيحة: A**

**س57:** What does the `lineTo(x, y)` method do in Canvas?
A) Moves the pen to (x,y) without drawing
B) Draws a line from the current point to (x,y)
C) Draws a line from the origin to (x,y)
D) Clears the canvas

**الإجابة الصحيحة: B**

**س58:** To close a path in Canvas (connect last point to first), you use:
A) endPath()
B) closePath()
C) finishPath()
D) stopPath()

**الإجابة الصحيحة: B**

---

## القسم السادس: التحويلات الهندسية (Transformations) - الأسئلة 59-80

**س59:** Which transformation moves points by a fixed distance in a given direction?
A) Scaling
B) Rotation
C) Translation
D) Shearing

**الإجابة الصحيحة: C**

**س60:** In 2D scaling, if sx = 2 and sy = 2, what happens to a point (1,1)?
A) It becomes (2,2)
B) It becomes (1,1)
C) It becomes (0.5,0.5)
D) It becomes (2,1)

**الإجابة الصحيحة: A**

**س61:** The rotation matrix for a counter-clockwise rotation by angle θ in 2D is:
A) `[[cosθ, sinθ], [-sinθ, cosθ]]`
B) `[[cosθ, -sinθ], [sinθ, cosθ]]`
C) `[[sinθ, cosθ], [cosθ, -sinθ]]`
D) `[[1, 0], [0, 1]]`

**الإجابة الصحيحة: B**

**س62:** Why are homogeneous coordinates used in transformation?
A) To make calculations slower
B) To represent translation as a matrix multiplication
C) To reduce the number of dimensions
D) To eliminate the need for scaling

**الإجابة الصحيحة: B**

**س63:** To rotate an object about an arbitrary point, the correct sequence is:
A) Rotate, translate, rotate
B) Translate to origin, rotate, translate back
C) Scale, rotate, translate
D) Translate, scale, rotate

**الإجابة الصحيحة: B**

**س64:** In 3D, the rotation matrix about the Z-axis is similar to 2D rotation with:
A) Z coordinate unchanged
B) X and Y swapped
C) Z set to zero
D) X and Z unchanged

**الإجابة الصحيحة: A** (Z remains same, X and Y transform)

**س65:** Which of the following is an affine transformation?
A) Translation
B) Scaling
C) Rotation
D) All of the above

**الإجابة الصحيحة: D**

**س66:** What is the result of reflecting the point (2,2) about the X-axis?
A) (2, -2)
B) (-2, 2)
C) (-2, -2)
D) (2, 2)

**الإجابة الصحيحة: A**

**س67:** In the shear transformation along the X-axis, which coordinate remains unchanged?
A) X coordinate
B) Y coordinate
C) Z coordinate (in 2D, Y remains unchanged)
D) Both X and Y change

**الإجابة الصحيحة: B**

**س68:** A 2D translation in homogeneous coordinates is represented by a:
A) 2x2 matrix
B) 3x3 matrix
C) 1x3 vector
D) 4x4 matrix

**الإجابة الصحيحة: B**

**س69:** To scale a triangle with vertices (1,1), (2,1), (1,3) by a factor of 2, the new coordinates of (1,3) become:
A) (2,6)
B) (3,5)
C) (2,2)
D) (4,2)

**الإجابة الصحيحة: A** (من مثال المحاضرة)

**س70:** Which method in HTML5 Canvas applies scaling, rotation, and translation in one step using a matrix?
A) setMatrix()
B) applyTransform()
C) transform()
D) matrix()

**الإجابة الصحيحة: C**

**س71:** In HTML5 Canvas, the `rotate()` method takes an angle in:
A) Degrees
B) Radians
C) Gradians
D) Turns

**الإجابة الصحيحة: B**

**س72:** What does the `scale(2,2)` method do in Canvas?
A) Moves the canvas by 2 pixels
B) Doubles the size of all subsequent drawings
C) Rotates the canvas by 2 radians
D) Clears the canvas

**الإجابة الصحيحة: B**

**س73:** To reflect an object about an arbitrary plane, the number of steps (translations and rotations) typically required is:
A) 2
B) 3
C) 5 (translate, rotate, mirror, reverse rotate, reverse translate)
D) 7

**الإجابة الصحيحة: C**

**س74:** In 3D rotation about the Y-axis, which row of the rotation matrix contains the sine terms with sign changes?
A) First row
B) Second row
C) Third row
D) Fourth row

**الإجابة الصحيحة: C** (الثالثة: [-sinβ, 0, cosβ, 0])

**س75:** The homogeneous coordinate for a 2D point (x,y) is usually represented as:
A) (x, y, 0)
B) (x, y, 1)
C) (x, y, w) where w can be any value
D) Both B and C are correct

**الإجابة الصحيحة: D** (w=1 للراحة، لكن w عموماً أي قيمة)

**س76:** A transformation that changes the size of an object is called:
A) Translation
B) Rotation
C) Scaling
D) Reflection

**الإجابة الصحيحة: C**

**س77:** The transformation matrix for 2D translation by (tx, ty) in homogeneous coordinates is:
A) `[[1,0,tx],[0,1,ty],[0,0,1]]`
B) `[[tx,0,0],[0,ty,0],[0,0,1]]`
C) `[[1,0,0],[0,1,0],[tx,ty,1]]`
D) `[[0,0,tx],[0,0,ty],[0,0,1]]`

**الإجابة الصحيحة: A** (أو حسب تنسيق الصف/العمود، لكن الشكل القياسي كما في المحاضرة)

**س78:** Which transformation matrix would produce a reflection about the Y-axis?
A) `[[-1,0,0],[0,1,0],[0,0,1]]`
B) `[[1,0,0],[0,-1,0],[0,0,1]]`
C) `[[0,1,0],[1,0,0],[0,0,1]]`
D) `[[-1,0,0],[0,-1,0],[0,0,1]]`

**الإجابة الصحيحة: A**

**س79:** In the composite transformation example for rotating a rectangle about its centroid, what is the first step?
A) Rotate the rectangle
B) Scale the rectangle
C) Translate the centroid to the origin
D) Translate the rectangle to the final position

**الإجابة الصحيحة: C**

**س80:** The `setTransform(a, b, c, d, e, f)` method in Canvas does what?
A) Adds the transformation to the existing one
B) Resets the current transformation and then applies the given matrix
C) Only reads the current transformation
D) Deletes all transformations

**الإجابة الصحيحة: B**

---

## القسم السابع: نماذج الألوان (Color Models) - الأسئلة 81-90

**س81:** Which color model is used for computer monitors and CRT displays?
A) CMYK
B) HSV
C) RGB
D) YIQ

**الإجابة الصحيحة: C**

**س82:** In the RGB color model, what color is produced by (1,1,1) in normalized values (assuming 1 is max)?
A) Black
B) White
C) Red
D) Cyan

**الإجابة الصحيحة: B**

**س83:** The CMYK color model is primarily used for:
A) Computer monitors
B) Color printers
C) Television broadcasting
D) User interface design

**الإجابة الصحيحة: B**

**س84:** What does "K" stand for in CMYK?
A) Key (black)
B) Kelvin
C) Kernel
D) Kyanite

**الإجابة الصحيحة: A**

**س85:** Which color model separates color into Hue, Saturation, and Value (Brightness)?
A) RGB
B) CMY
C) YIQ
D) HSV

**الإجابة الصحيحة: D**

**س86:** The YIQ color model was developed for:
A) European television
B) US commercial color TV broadcasting (NTSC)
C) Digital cameras
D) Printers

**الإجابة الصحيحة: B**

**س87:** In the additive color model (RGB), combining red and green light produces:
A) Yellow
B) Cyan
C) Magenta
D) White

**الإجابة الصحيحة: A**

**س88:** In the subtractive color model (CMYK), combining cyan and magenta inks on white paper should theoretically produce:
A) Red
B) Blue
C) Green
D) Black (or dark muddy color)

**الإجابة الصحيحة: B** (Cyan يطرح الأحمر، Magenta يطرح الأخضر -> يتبقى الأزرق)

**س89:** The wavelength range for visible light is approximately:
A) 100-300 nm
B) 400-700 nm
C) 700-1000 nm
D) 1-100 nm

**الإجابة الصحيحة: B**

**س90:** Which method in HTML5 Canvas creates a linear gradient?
A) createGradient()
B) createLinearGradient(x1, y1, x2, y2)
C) linearGradient(color1, color2)
D) addGradient()

**الإجابة الصحيحة: B**
