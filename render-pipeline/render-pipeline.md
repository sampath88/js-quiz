# Rendering Pipeline & Compositing

#### 1. Parse HTML & Generate DOM Tree
![Alt text](image.png)

#### 2. Parse CSS & Generate CSSOM Tree
![Alt text](image-1.png)

#### 3. Render Tree
![Alt text](image-2.png)

It creates Render Tree by combining both DOM tree and CSSOM tree,
It only includes the visual elements which we actually see on the screen.
The Render Tree contains both the styles and HTML
- Note: It doesn't include elements like 'head','script', display hidden elements.

#### 4. Layout Process
![Alt text](image-3.png)

#### 5. Paint Phase
![Alt text](image-4.png)
Paint process assings colors and images to the visual elements in the render tree

#### 6. Composite
![Alt text](image-5.png)

Combines all the layers. The Composite process happens on the compositor thread. It's like separate thread in GPU.

#### 7. Display on screen
![Alt text](image-6.png)