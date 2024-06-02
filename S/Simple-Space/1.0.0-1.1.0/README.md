# Comparing `tmp/simple_space-1.0.0.tar.gz` & `tmp/simple_space-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-1.0.0.tar", last modified: Sat Jun  1 08:49:36 2024, max compression
+gzip compressed data, was "simple_space-1.1.0.tar", last modified: Sun Jun  2 18:32:34 2024, max compression
```

## Comparing `simple_space-1.0.0.tar` & `simple_space-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11235 2024-06-01 08:49:36.876934 simple_space-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10162 2024-06-01 07:21:16.000000 simple_space-1.0.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/SimpleS/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/SimpleS/ImageRelated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-1.0.0/SimpleS/ImageRelated/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10405 2024-06-01 08:46:42.000000 simple_space-1.0.0/SimpleS/ImageRelated/basics.py
--rw-r--r--   0 user      (1000) user      (1000)     4425 2024-05-31 18:38:19.000000 simple_space-1.0.0/SimpleS/ImageRelated/enhancements.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/SimpleS/Points/
--rw-rw-r--   0 user      (1000) user      (1000)    10560 2024-06-01 08:43:06.000000 simple_space-1.0.0/SimpleS/Points/Circle.py
--rw-rw-r--   0 user      (1000) user      (1000)     4137 2024-06-01 08:43:22.000000 simple_space-1.0.0/SimpleS/Points/Line.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-1.0.0/SimpleS/Points/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4751 2024-05-31 18:21:41.000000 simple_space-1.0.0/SimpleS/Points/dim2.py
--rw-rw-r--   0 user      (1000) user      (1000)     7887 2024-06-01 08:46:46.000000 simple_space-1.0.0/SimpleS/Points/dim3.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 22:02:16.000000 simple_space-1.0.0/SimpleS/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1476 2024-05-31 18:22:46.000000 simple_space-1.0.0/SimpleS/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/Simple_Space.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11235 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      470 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-06-01 08:49:22.000000 simple_space-1.0.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-06-01 08:49:36.876934 simple_space-1.0.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-02 18:32:34.433928 simple_space-1.1.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-1.1.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11235 2024-06-02 18:32:34.433928 simple_space-1.1.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    10162 2024-06-01 07:21:16.000000 simple_space-1.1.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-02 18:32:34.425928 simple_space-1.1.0/SimpleS/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-02 18:32:34.425928 simple_space-1.1.0/SimpleS/ImageRelated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-1.1.0/SimpleS/ImageRelated/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10587 2024-06-02 18:26:27.000000 simple_space-1.1.0/SimpleS/ImageRelated/basics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4425 2024-05-31 18:38:19.000000 simple_space-1.1.0/SimpleS/ImageRelated/enhancements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-02 18:32:34.429928 simple_space-1.1.0/SimpleS/Points/
+-rw-rw-r--   0 user      (1000) user      (1000)    12145 2024-06-02 00:47:59.000000 simple_space-1.1.0/SimpleS/Points/Circle.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15635 2024-06-02 00:58:00.000000 simple_space-1.1.0/SimpleS/Points/Line.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4655 2024-06-02 01:16:45.000000 simple_space-1.1.0/SimpleS/Points/Triangle.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-1.1.0/SimpleS/Points/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4986 2024-06-02 00:58:02.000000 simple_space-1.1.0/SimpleS/Points/dim2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8096 2024-06-01 17:18:38.000000 simple_space-1.1.0/SimpleS/Points/dim3.py
+-rw-rw-r--   0 user      (1000) user      (1000)       28 2024-06-02 17:30:39.000000 simple_space-1.1.0/SimpleS/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5275 2024-06-02 17:30:06.000000 simple_space-1.1.0/SimpleS/detection.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1476 2024-05-31 18:22:46.000000 simple_space-1.1.0/SimpleS/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-02 18:32:34.433928 simple_space-1.1.0/Simple_Space.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11235 2024-06-02 18:32:34.000000 simple_space-1.1.0/Simple_Space.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      518 2024-06-02 18:32:34.000000 simple_space-1.1.0/Simple_Space.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-06-02 18:32:34.000000 simple_space-1.1.0/Simple_Space.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2024-06-02 18:32:34.000000 simple_space-1.1.0/Simple_Space.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2024-06-02 18:32:34.000000 simple_space-1.1.0/Simple_Space.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-06-02 18:26:57.000000 simple_space-1.1.0/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-06-02 18:32:34.433928 simple_space-1.1.0/setup.cfg
```

### Comparing `simple_space-1.0.0/LICENSE` & `simple_space-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_space-1.0.0/PKG-INFO` & `simple_space-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-1.0.0/README.md` & `simple_space-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_space-1.0.0/SimpleS/ImageRelated/basics.py` & `simple_space-1.1.0/SimpleS/ImageRelated/basics.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,74 +187,67 @@
         img = ndi.gaussian_filter(img.astype(float), sigma=1)
         img = img > 0.5
         
         return img
 
 
 def detect_edges(image, 
+                 detection_distance_start = 5,
+                 detection_distance_end = 10,
+                 how_many_detection = 4,
                  n1=100, 
                  n2=100,  
                  show_edges = True, 
                  show_contours=True, 
                  title_for_detected_edges = 'Detected Edges',
                  title_for_detected_contours = 'Detected Edges with Contours',
                  return_edges = False, 
                  return_contours = False, 
-                 range_color_start=100, 
-                 range_color_end=255, 
                  save = False,
                  save_path = None,
                  file_name = None):
-    
     if isinstance(image, str):
         image = cv2.imread(image, cv2.IMREAD_GRAYSCALE)
         if image is None:
             raise ValueError(f"Image file '{image}' not found or could not be read.")
     elif isinstance(image, np.ndarray):
         if len(image.shape) != 2:
             raise ValueError("Image must be a grayscale image.")
     else:
         raise TypeError("Input must be a file path (str) or a grayscale image (numpy.ndarray).")
-    
     blurred_image = cv2.GaussianBlur(image, (5, 5), 0)
-    
+    _, binary_image_pure = cv2.threshold(image, 127, 255, cv2.THRESH_BINARY)
     _, binary_image = cv2.threshold(blurred_image, 127, 255, cv2.THRESH_BINARY)
-    
+    dist_transform = cv2.distanceTransform(binary_image_pure, cv2.DIST_L2, 5)
     kernel = np.ones((5, 5), np.uint8)
     closed_image = cv2.morphologyEx(binary_image, cv2.MORPH_CLOSE, kernel)
-    
     edges = cv2.Canny(closed_image, n1, n2, apertureSize=3)
     if show_edges:
         plt.imshow(edges, cmap='gray')
         plt.title(title_for_detected_edges)
         plt.axis('off')
         plt.show()
     if save:
         path_to_save = save_path_generator(file_name, save_path, flag = 'DetectedEdges')
         plt.imsave(path_to_save, edges)
-    contours, _ = cv2.findContours(edges, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
-    canvas = np.zeros_like(image)
-    for contour in contours:
-        color = np.random.randint(range_color_start, range_color_end, size=3, dtype=np.uint8)
-        color = tuple(map(int, color))
-        cv2.drawContours(canvas, [contour], -1, color, 2)
-    
-    canvas_rgb = cv2.cvtColor(canvas, cv2.COLOR_GRAY2BGR)
-    canvas_rgb = cv2.cvtColor(canvas_rgb, cv2.COLOR_BGR2RGB)
-    if show_contours:
-        plt.imshow(canvas_rgb)
-        plt.title(title_for_detected_contours)
-        plt.axis('off')
-        plt.show()
-    if save:
-        path_to_save = save_path_generator(file_name, save_path, flag = 'DetectedContours')
-        plt.imsave(path_to_save, canvas_rgb)
-    
+    for dd in np.linspace(start=detection_distance_start, stop=detection_distance_end, num=how_many_detection):
+        contours, _ = cv2.findContours((dist_transform >= dd).astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+        contour_img = np.zeros_like(dist_transform)
+        for contour in contours:
+            cv2.drawContours(contour_img, [contour], -1, (255), 1)
+        if show_contours:
+            plt.imshow(contour_img)
+            plt.title(f"{title_for_detected_contours} at Distance =  {dd}")
+            plt.axis('off')
+            plt.show()
+        if save:
+            path_to_save = save_path_generator(file_name, save_path, flag = f'DetectedContours_dist{dd}')
+            plt.imsave(path_to_save, contour_img)
     if return_edges and return_contours:
-        return edges, canvas
+        return edges, contour_img
     elif return_edges:
         return edges
     elif return_contours:
-        return canvas
+        return contour_img
     else:
         return
 #end#
```

### Comparing `simple_space-1.0.0/SimpleS/ImageRelated/enhancements.py` & `simple_space-1.1.0/SimpleS/ImageRelated/enhancements.py`

 * *Files identical despite different names*

### Comparing `simple_space-1.0.0/SimpleS/Points/Circle.py` & `simple_space-1.1.0/SimpleS/Points/Circle.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 #In the name of God # #
 #
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy.spatial import ConvexHull
-
+from numpy.polynomial import Polynomial
 
 
 def plot_circles_along_arc(center, radius, start_angle, end_angle, circle_radius):
     """
     Plots circles along a circular arc.
     Parameters:
     - center: Tuple (x, y), the center of the arc
     - radius: Radius of the arc
     - start_angle, end_angle: Angles in degrees defining the arc
     - circle_radius: Radius of the circles to plot along the arc
     """
     fig, ax = plt.subplots()
     start_angle = np.deg2rad(start_angle)
     end_angle = np.deg2rad(end_angle)
-    # Calculate limit of circles for fit along the arc
+    #circles for fit along the arc
     arc_length = radius * (end_angle - start_angle)
     number_of_circles = int(arc_length / (2 * circle_radius))
     angle_increment = (end_angle - start_angle) / number_of_circles
-    # Plot each circle along the arc
     for i in range(number_of_circles + 1):
         angle = start_angle + i * angle_increment
         circle_center = (center[0] + (radius - circle_radius) * np.cos(angle),
                          center[1] + (radius - circle_radius) * np.sin(angle))
         circle = plt.Circle(circle_center, circle_radius, color='r', fill=False, lw=2)
         ax.add_patch(circle)
     #arc = plt.Arc(center, 2 * radius, 2 * radius, angle=0, theta1=np.rad2deg(start_angle), theta2=np.rad2deg(end_angle), color='blue', linestyle='--')
@@ -50,18 +48,17 @@
     float: angle in degrees.
     """
     center = np.array(center)
     start_point = np.array(start_point)
     end_point = np.array(end_point)
     vector1 = start_point - center
     vector2 = end_point - center
-    # Calculate angles using atan2
+    #angles using atan2
     angle1 = np.arctan2(vector1[1], vector1[0])
     angle2 = np.arctan2(vector2[1], vector2[0])
-    # ensure a positive angle
     angle = angle2 - angle1
     if angle < 0:
         angle += 2 * np.pi
     return np.degrees(angle)
 
 
 def calculate_circle_center(p1, p2, p3):
@@ -76,15 +73,15 @@
     p2 = np.array(p2)
     p3 = np.array(p3)
     mid1 = (p1 + p2) / 2
     mid2 = (p2 + p3) / 2
     # slopes of lines p1p2 and p2p3
     slope1 = (p2[1] - p1[1]) / (p2[0] - p1[0]) if p2[0] != p1[0] else float('inf')
     slope2 = (p3[1] - p2[1]) / (p3[0] - p2[0]) if p3[0] != p2[0] else float('inf')
-    # handle vertical lines
+    # vertical lines
     if slope1 == float('inf'):
         center_x = mid1[0]
         center_y = mid2[1] + (mid2[0] - center_x) / slope2
     elif slope2 == float('inf'):
         center_x = mid2[0]
         center_y = mid1[1] + (mid1[0] - center_x) / slope1
     else:
@@ -103,16 +100,65 @@
         Example: t=0.5t=0.5 gives you the midpoint of the curve.
     """
     while len(points) > 1:
         points = [p1 + t * (p2 - p1) for p1, p2 in zip(points[:-1], points[1:])]
     return points[0]
 
 
+def create_and_fit_curve_with_points(x_points, y_points, degree):
+    """
+    Fit a polynomial curve to the given data points and return the polynomial equation.
+    Args:
+    x_points (list): List of x-coordinates of the data points.
+    y_points (list): List of y-coordinates of the data points.
+    degree (int): Degree of the polynomial to fit.
+    Returns:
+    Polynomial: The fitted polynomial.
+    """
+    coefs = np.polyfit(x_points, y_points, degree)  # returns coefs in reverse order
+    poly = Polynomial(coefs[::-1])
+    return poly
+
+
+def plot_a_curve(x_points, y_points, degree):
+    """
+    Plot a curve by creating a new figure and axes.
+    Args:
+    x_points (list): List of x-coordinates of the data points.
+    y_points (list): List of y-coordinates of the data points.
+    degree (int): Degree of the polynomial to fit.
+    """
+    poly = create_and_fit_curve_with_points(x_points, y_points, degree)
+    x_new = np.linspace(min(x_points), max(x_points), 500)
+    y_new = poly(x_new)
+    fig, ax = plt.subplots()
+    ax.plot(x_points, y_points, 'o', label='Data points')
+    ax.plot(x_new, y_new, '-', label=f'Polynomial fit (degree {degree})')
+    ax.legend()
+    plt.show()
+
+
+def plot_curve_on_given_ax(ax, x_points, y_points, degree):
+    """
+    Plot a curve on an existing axes.
+    Args:
+    ax (matplotlib.axes.Axes): Existing matplotlib axes to plot on.
+    x_points (list): List of x-coordinates of the data points.
+    y_points (list): List of y-coordinates of the data points.
+    degree (int): Degree of the polynomial to fit.
+    """
+    poly = create_and_fit_curve_with_points(x_points, y_points, degree)
+    x_new = np.linspace(min(x_points), max(x_points), 500)
+    y_new = poly(x_new)
+    ax.plot(x_points, y_points, 'o', label='Data points')
+    ax.plot(x_new, y_new, '-', label=f'Polynomial fit (degree {degree})')
+    ax.legend()
+
+
 def bezier_tangent(t, points):
-    
     """ Calculate the tangent to the curve at parameter t. """
     derivative_points = [n * (p2 - p1) for n, (p1, p2) in enumerate(zip(points[:-1], points[1:]), 1)]
     return position_of_point_along_curve(t, derivative_points)
 
 
 def angle_between_tangents(t1, t2, control_points):
     """ Calculate the angle between the tangents at two points along a Bezier curve."""
@@ -127,26 +173,21 @@
     Plots a series of tangent circles between two points with specified radius.
     Assumes a straight line path between start and end points.
     """
     fig, ax = plt.subplots()
     # Calculate the distance between the start and end points
     distance = np.linalg.norm(end_point - start_point)
     direction = (end_point - start_point) / distance
-    
     # Calculate positions of circle centers
     centers = [start_point + direction * radius * (1 + 2 * i) for i in range(num_circles)]
-    
-    # Plotting each circle
     for center in centers:
         circle = plt.Circle(center, radius, color='r', fill=False, lw=2)
         ax.add_patch(circle)
-    # Drawing the line for reference
     line = np.vstack([start_point, end_point])
     plt.plot(line[:,0], line[:,1], 'b--')
-    # Set limits and aspect
     ax.set_xlim(min(start_point[0], end_point[0]) - radius, max(start_point[0], end_point[0]) + radius)
     ax.set_ylim(min(start_point[1], end_point[1]) - radius, max(start_point[1], end_point[1]) + radius)
     ax.set_aspect('equal')
     plt.grid(True)
     plt.show()
 
 
@@ -155,32 +196,28 @@
     Plots circles tangent to two horizontal lines from start_x to end_x.
     The circles' diameters are determined by the distance between lower_y and upper_y.
     """
     radius = (upper_y - lower_y) / 2
     center_y = (upper_y + lower_y) / 2
     number_of_circles = int((end_x - start_x) / (2 * radius))
     fig, ax = plt.subplots()
-    
     ax.hlines(y=[lower_y, upper_y], xmin=start_x, xmax=end_x, color='blue', linestyle='--')
-    
     for i in range(number_of_circles):
         center_x = start_x + radius + i * 2 * radius
         circle = plt.Circle((center_x, center_y), radius, color='r', fill=False, lw=2)
         ax.add_patch(circle)
     ax.set_xlim(start_x - 1, end_x + 1)
     ax.set_ylim(lower_y - 1, upper_y + 1)
     ax.set_aspect('equal')
     plt.grid(True)
     plt.show()
 
-
 def midpoint(p1, p2):
     return (p1 + p2) / 2
 
-
 def perpendicular_bisector(p1, p2):
     # Returns the slope and intercept of the perpendicular bisector
     if p2[0] - p1[0] == 0:  # vertical line
         return None, p1[0]
     elif p2[1] - p1[1] == 0:  # horizontal line
         return 0, p1[1]
     else:
@@ -189,16 +226,16 @@
         intercept = midpoint[1] - slope * midpoint[0]
         return slope, intercept
 
 
 def find_smallest_circle(points):
     # Helper function to calculate the circle from three points
     def calculate_circle(p1, p2, p3):
-        # Calculate the circumscribed circle of the triangle formed by points p1, p2, p3
-        # Using determinant method
+        # circle of the triangle formed by points p1, p2, p3
+        # determinant method
         A = np.linalg.det([[p1[0], p1[1], 1],
                            [p2[0], p2[1], 1],
                            [p3[0], p3[1], 1]])
         B = np.linalg.det([[p1[0]**2 + p1[1]**2, p1[1], 1],
                            [p2[0]**2 + p2[1]**2, p2[1], 1],
                            [p3[0]**2 + p3[1]**2, p3[1], 1]])
         C = np.linalg.det([[p1[0]**2 + p1[1]**2, p1[0], 1],
@@ -226,30 +263,29 @@
             for k in range(j + 1, len(points)):
                 center, radius = calculate_circle(points[i], points[j], points[k])
                 if radius < smallest_radius:
                     valid = all(np.linalg.norm(center - p) <= radius + 1e-12 for p in points)
                     if valid:
                         smallest_radius = radius
                         smallest_circle = (center, radius)
-    # In case no valid circle was found with three points, fallback to any two points
+    #fallback to any two points if no valid circle was found
     if smallest_circle is None:
         for i in range(len(points)):
             for j in range(i + 1, len(points)):
                 mid_point = (points[i] + points[j]) / 2
                 radius = np.linalg.norm(points[i] - mid_point)
                 if radius < smallest_radius:
                     smallest_radius = radius
                     smallest_circle = (mid_point, radius)
     return smallest_circle
 
 
 def plot_polygon_with_circle(points, 
                              circle, fill_circle = None, lw_circle = 1, circle_color = 'r',
                              edgecolor='black', fill_edge=None,  lw_edge=1):
-    
     polygon = plt.Polygon(points, edgecolor=edgecolor, fill=fill_edge, lw=lw_edge)
     fig, ax = plt.subplots()
     ax.add_patch(polygon)
     if circle:
         center, radius = circle
         circle_patch = plt.Circle(center, radius, color=circle_color, fill=fill_circle, lw=lw_circle)
         ax.add_patch(circle_patch)
```

### Comparing `simple_space-1.0.0/SimpleS/Points/dim2.py` & `simple_space-1.1.0/SimpleS/Points/dim2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-
+#in the name of GOD##
 import os
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 from SimpleS.utils import save_path_generator
 import scipy.ndimage as ndi
 from skimage import img_as_ubyte
 from skimage.morphology import skeletonize
 
 
+def calculate_midpoint(A, B):
+    """Calculate the midpoint between two points A and B."""
+    x1, y1 = A
+    x2, y2 = B
+    mid_x = (x1 + x2) / 2
+    mid_y = (y1 + y2) / 2
+    return (mid_x, mid_y)
 
 
 def rotate_2d_points(points, theta=0, axis=None):
     """Rotate or reflect 2D points by theta degrees around the origin or inverting the specified axis."""
     points = np.asarray(points)
     if points.shape[1] != 2:
         raise ValueError("Points should be in shape (n, 2)")
@@ -31,38 +38,39 @@
     else:
         # rotation around the origin by theta.
         theta = np.radians(theta)
         rot_matrix = np.array([
             [np.cos(theta), -np.sin(theta)],
             [np.sin(theta), np.cos(theta)]
         ])
+    
     return np.dot(points, rot_matrix.T)
 
 
-
-
 def create_flat_image(size=(750, 750), color_mode='RGB', color = 'White',return_ = True, save = False, save_path = None, file_name = None):
         """
-        Create a white image of the specified size and color mode.
+        Create an image of the specified size and color mode.
         Parameters:
         size (tuple): The dimensions of the image (width, height).
         color_mode (str): The color mode of the image, either 'RGB' or 'Gray'.
         Returns:
         numpy.ndarray: The created white image.
         """
         col = 255 if color.lower() == 'white' else 0
+        
         if color_mode.lower() == 'rgb':
                 image = np.ones((size[1], size[0], 3), dtype=np.uint8) * col
         elif color_mode.lower() == 'gray':
                 image = np.ones((size[1], size[0]), dtype=np.uint8) * col
         else:
                 raise ValueError("Invalid color mode. Choose 'RGB' or 'Gray'.")
         if save:
                 path_to_save = save_path_generator(file_name, save_path, flag=f'{size}_{color}')
                 plt.imsave(path_to_save, image)
+        
         if return_:
                 return image
         else:
                 return
 
 
 def detect_centerline(image,
@@ -122,8 +130,8 @@
                 plt.show()
         else:
                 if save and not silently:
                         print(f"Result is Saved in {save_path}")
                         return
                 else:
                         return
-#end#
+#end#
```

### Comparing `simple_space-1.0.0/SimpleS/Points/dim3.py` & `simple_space-1.1.0/SimpleS/Points/dim3.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 from SimpleS.utils import save_path_generator
 
 
 
 def read_off_file(file_path):
-        """ It will return 2Object  Vertices  and  Faces. """
+        """ It will return bject's Vertices  and  Faces. """
         with open(file_path, 'r') as file:
                 if file.readline().strip() != "OFF":
                         raise ValueError("Not a valid OFF file")
                 n_vertices, n_faces, _ = map(int, file.readline().strip().split())
                 vertices = [tuple(map(float, file.readline().strip().split())) for _ in range(n_vertices)]
                 faces = [tuple(map(int, file.readline().strip().split()[1:])) for _ in range(n_faces)]
                 vertices = np.asarray(vertices)
                 print("Secssesful . Vertices")
                 faces = np.asarray(faces)
                 print("Secssesful . Faces")
         
         return vertices, faces
+
+
+def read_pts_file(file_path):
     
+    with open(file_path, 'r') as file:
+        points = [tuple(map(float, line.strip().split())) for line in file.readlines()]
+    print("Secssesful . Points from the PTS file.")
     
+    return points
+
 
 def rotate_3d_points(points, theta, axis='z'):
         """Rotate 3D points around the specified axis by theta degrees."""
         theta = np.radians(theta)
         if axis == 'x':
                 rot_matrix = np.array([
                         [1, 0, 0],
@@ -41,16 +49,15 @@
                 rot_matrix = np.array([
                         [np.cos(theta), -np.sin(theta), 0],
                         [np.sin(theta), np.cos(theta), 0],
                         [0, 0, 1]
                 ])
         
         return np.dot(points, rot_matrix.T)
-    
-    
+
 
 def plot_3d_points_using_vertices(v, f=None, axis = 'on', title = '3D Data Visualization', faces_colors = 'blue', alpha=0.75, linewidths=1, edgecolors='r', point_color='blue',show =True, save=False, save_path = None, file_name = None ):
         """
         Plot 3D points or a mesh from vertices and optionally faces.
         
         Parameters:
         - v: List of vertices where each vertex is a list or tuple [x, y, z].
@@ -99,16 +106,15 @@
                 plt.savefig(path_to_save_file)
         if show:
                 plt.show()
         else:
                 plt.clf()
                 plt.close()
                 return
-    
-    
+
 
 def create_bool_image_from_3d_points(points, image_size=(500, 500),save = False, save_path = None, file_name = None):
         """
         Create a grayscale image from 3D points by projecting them onto a 2D plane using the z-coordinate
         as intensity.
         Args:
         points (numpy.ndarray): An array of points with shape (N, 3), where each row represents a 3D point (x, y, z).
@@ -166,9 +172,8 @@
                 plt.axis('off')
         ax.set_title(title)
         plt.show()
         if save:
                 path_to_save = save_path_generator(file_name, save_path, flag=None)
                 print(f"Plot saved to {path_to_save}")
 
-#end#
-
+#end#
```

### Comparing `simple_space-1.0.0/SimpleS/utils.py` & `simple_space-1.1.0/SimpleS/utils.py`

 * *Files identical despite different names*

### Comparing `simple_space-1.0.0/Simple_Space.egg-info/PKG-INFO` & `simple_space-1.1.0/Simple_Space.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-1.0.0/pyproject.toml` & `simple_space-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Space"
-version = "1.0.0"
+version = "1.1.0"
 description = "A Try at Better Understanding Space."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
```

