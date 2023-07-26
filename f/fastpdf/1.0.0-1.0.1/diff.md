# Comparing `tmp/fastpdf-1.0.0.tar.gz` & `tmp/fastpdf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastpdf-1.0.0.tar", last modified: Wed Jul 26 07:11:45 2023, max compression
+gzip compressed data, was "fastpdf-1.0.1.tar", last modified: Wed Jul 26 07:15:24 2023, max compression
```

## Comparing `fastpdf-1.0.0.tar` & `fastpdf-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:11:45.247278 fastpdf-1.0.0/
--rw-rw-r--   0 ko        (1000) ko        (1000)    13814 2023-07-26 07:11:45.247278 fastpdf-1.0.0/PKG-INFO
--rw-rw-r--   0 ko        (1000) ko        (1000)    13196 2023-07-17 15:26:34.000000 fastpdf-1.0.0/README.md
-drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:11:45.247278 fastpdf-1.0.0/fastpdf/
--rw-rw-r--   0 ko        (1000) ko        (1000)       68 2023-06-29 11:16:02.000000 fastpdf-1.0.0/fastpdf/__init__.py
--rw-rw-r--   0 ko        (1000) ko        (1000)    36041 2023-07-17 15:11:41.000000 fastpdf-1.0.0/fastpdf/api.py
--rw-rw-r--   0 ko        (1000) ko        (1000)      671 2023-06-29 11:15:01.000000 fastpdf-1.0.0/fastpdf/exceptions.py
--rw-rw-r--   0 ko        (1000) ko        (1000)     4015 2023-07-19 11:30:28.000000 fastpdf-1.0.0/fastpdf/models.py
-drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:11:45.247278 fastpdf-1.0.0/fastpdf.egg-info/
--rw-rw-r--   0 ko        (1000) ko        (1000)    13814 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/PKG-INFO
--rw-rw-r--   0 ko        (1000) ko        (1000)      247 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/SOURCES.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)        1 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/dependency_links.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)       22 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/requires.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)        8 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/top_level.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)       38 2023-07-26 07:11:45.247278 fastpdf-1.0.0/setup.cfg
--rw-rw-r--   0 ko        (1000) ko        (1000)     1026 2023-07-26 07:11:41.000000 fastpdf-1.0.0/setup.py
+drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:15:24.722416 fastpdf-1.0.1/
+-rw-rw-r--   0 ko        (1000) ko        (1000)    12972 2023-07-26 07:15:24.722416 fastpdf-1.0.1/PKG-INFO
+-rw-rw-r--   0 ko        (1000) ko        (1000)    12354 2023-07-26 07:15:02.000000 fastpdf-1.0.1/README.md
+drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:15:24.722416 fastpdf-1.0.1/fastpdf/
+-rw-rw-r--   0 ko        (1000) ko        (1000)       68 2023-06-29 11:16:02.000000 fastpdf-1.0.1/fastpdf/__init__.py
+-rw-rw-r--   0 ko        (1000) ko        (1000)    36041 2023-07-17 15:11:41.000000 fastpdf-1.0.1/fastpdf/api.py
+-rw-rw-r--   0 ko        (1000) ko        (1000)      671 2023-06-29 11:15:01.000000 fastpdf-1.0.1/fastpdf/exceptions.py
+-rw-rw-r--   0 ko        (1000) ko        (1000)     4015 2023-07-19 11:30:28.000000 fastpdf-1.0.1/fastpdf/models.py
+drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:15:24.722416 fastpdf-1.0.1/fastpdf.egg-info/
+-rw-rw-r--   0 ko        (1000) ko        (1000)    12972 2023-07-26 07:15:24.000000 fastpdf-1.0.1/fastpdf.egg-info/PKG-INFO
+-rw-rw-r--   0 ko        (1000) ko        (1000)      247 2023-07-26 07:15:24.000000 fastpdf-1.0.1/fastpdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)        1 2023-07-26 07:15:24.000000 fastpdf-1.0.1/fastpdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)       22 2023-07-26 07:15:24.000000 fastpdf-1.0.1/fastpdf.egg-info/requires.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)        8 2023-07-26 07:15:24.000000 fastpdf-1.0.1/fastpdf.egg-info/top_level.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)       38 2023-07-26 07:15:24.722416 fastpdf-1.0.1/setup.cfg
+-rw-rw-r--   0 ko        (1000) ko        (1000)     1026 2023-07-26 07:15:08.000000 fastpdf-1.0.1/setup.py
```

### Comparing `fastpdf-1.0.0/PKG-INFO` & `fastpdf-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: fastpdf
-Version: 1.0.0
-Summary: SDK for PDF rendering, generation & transformation via Fast PDF Service.
-Home-page: https://github.com/fastpdfservices/fastpdf-python
-Author: Korian
-Author-email: korian@fastpdfservice.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
 # FastPDF Python Package
 
 Welcome to **fastpdf** Python Package, the versatile and quick solution for your PDF rendering needs. This package is a SDK for fastpdfservice.com REST API.
 
 ## Overview
 
 `fastpdf` is a Python package designed to simplify the PDF generation process. It streamlines the procedure of rendering HTML/CSS templates into a PDF document, offering granular control over the rendering options, and provides the ability to add images and barcodes into your PDFs.
@@ -50,85 +33,74 @@
 from fastpdf import PDFClient
 ```
 
 To start with, make sure you have your FastPDF service API token handy. 
 This is required for all API calls to the FastPDF service. You can find your token under API settings in 
 your [FastPDF profile](https://fastpdfservice.com/profile/api).
 
-<CodeGroup title="Register your token">
 
 ```python {{ title: 'Python' }}
 client = PDFClient("API_KEY")
 ```
 
-</CodeGroup>
-
-
 Please refer to the [documentation](https://docs.fastpdfservice.com) for more details on the available features.
 
 
 ## Creating a Basic Template
 
 Creating a basic template is simple. Let's start by creating an HTML document with a placeholder for a `name` variable.
-Then, you'll need to create a [Template](templates#template) object and set `name` and `format`.
-
+Then, you'll need to create a [Template](https://docs.fastpdfservice.com/templates#template) object and set `name` and `format`.
 
-<CodeGroup title="Creating a basic template">
 
 ```python {{ title: 'Python' }}
 from fastpdf import Template
 
 template_str = "<html><body>Hello world, my name is {{name}}!</body></html>".encode()
 template_data = Template(name="basic-document", format="html")
 template = client.add_template(template_str, template_data)
 ```
 
-</CodeGroup>
 
 <Note>
-  Make sure you do not forget to `encode()` your string. Otherwise, the string will be interpreted as a filename.
+  *Make sure you do not forget to `encode()` your string. Otherwise, the string will be interpreted as a filename.*
 </Note>
 
 In this template, `{{name}}` is a placeholder that will be replaced by a real value when generating a PDF. 
 
 ## Your First Rendering
 
 Now, let's bring our document to life. We've got our template id handy, and our data ready to be cast into the chosen template. 
 But don't worry if you've misplaced the template id - a quick detour to your [template dashboard](https://fastpdfservice.com/services/templates) will point you right to it.
 In our data object, we set a value for the `name` variable that we defined in our template.
 
-<CodeGroup title="Rendering our basic template">
 
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 'name': 'John' }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
 ```
 
-</CodeGroup>
 
 Finally, we save it to the disk using the `save()` convenience function.
 
-<CodeGroup title="Saving our document to the disk">
 
 ```python {{ title: 'Python' }}
 client.save(document, "path/to/basic-document.pdf")
 ```
 
-</CodeGroup>
 
 And that's it! You've just brought your first PDF to life.
 
 
 ## For Loops
 
 FastPDF allows for more complex templates. For instance, you can use control structures like for loops and if statements in your templates.
 Here is how to iterate over a list of items, using a for loop.
 
-<CodeGroup title="For Loop">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <ul>
     {% for item in items %}
@@ -138,38 +110,34 @@
 </body>
 </html>
 """.encode()
 template_data = Template(name="for-loop-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 In this template, `{% for item in items %}` starts the loop, and `{% endfor %}` ends it.
 
 Next, we define our rendering_data by associating a list of item value to the `items` key, and render our document.
 
-<CodeGroup title="Rendering our For Loop template">
-
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 'items': ["First item", "Second item", "Last item"] }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
+# Save to disk, if needed
 client.save(document, "path/to/loop-document.pdf")
 ```
 
-</CodeGroup>
 
 
 ## If Statements
 
 If statements can be used to conditionally include parts of the template, based on the rendering data. Here's an example:
 
-<CodeGroup title="If statement">
-
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     {% if user_premium %}
         <p>Welcome, premium user!</p>
     {% else %}
@@ -178,34 +146,32 @@
 </body>
 </html>
 """.encode()
 template_data = Template(name="if-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 In this example, `{% if user_premium %}` starts the if statement, and `{% endif %}` ends it. 
 If `user_premium` is true, the "Welcome, premium user!" message will be included in the generated PDF. 
 Otherwise, the "Welcome, regular user!" message will be included.
 
 ## Stylesheets
 
 <Note>
-    Please ensure that your stylesheets are written purely in CSS. As of now, FastPDF does not support precompiled CSS languages 
+    *Please ensure that your stylesheets are written purely in CSS. As of now, FastPDF does not support precompiled CSS languages 
     like SCSS, or CSS frameworks like Tailwind. 
-    Stick to standard CSS to ensure compatibility and successful rendering.
+    Stick to standard CSS to ensure compatibility and successful rendering.*
 </Note>
 
 You can do this in one of two ways: by using a separate stylesheet, or by using inline CSS. 
 
 The latter works as usual, by either
 setting the `style` property html tags, or by writing your css classes in the header of the template:
 
-<CodeGroup title="A template with style">
 
 ```html {{ title: 'HTML' }}
 <html>
 <head>
     my-class {
         color: #f43f54;
         font-size: 12px;
@@ -215,120 +181,109 @@
 <body>
     <p class='my-class'>Welcome, {{name}}!</p>
     <p style='color: #ccc'> Goodbye ! </p>
 </body>
 </html>
 ```
 
-</CodeGroup>
-
 Alternatively, you can use the `add_stylesheet()` method to add a stylesheet to your template:
 
-<CodeGroup title="A template with style">
 
 ```python {{ title: 'Python' }}
 from fastpdf import StylesheetFile
 
 stylesheet_path = "styles.css"
 stylesheet_data = StylesheetFile(format="css")
+
 template_id = template["id"]
 client.add_stylesheet(template_id, stylesheet_path, stylesheet_data)
-
 ```
 
-</CodeGroup>
 
 Your template will now be rendered with style !
 
 ## Adding an image
 
 FastPDF allows you to add images to your templates, which can then be rendered into your final PDF documents. Here's how you can accomplish this.
 
 To begin, we create our template with an `<img>` tag, using our image uri in the `src` property as followed:
 
-<CodeGroup title="Creating a template with an image">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <img src="{{my_favourite_logo}}">
     <p>Welcome, {{name}}!</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="image-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 Then, we add an image to our template, and set the same image uri. 
 This step can be done from your [template dashboard](https://fastpdfservice.com/services/templates).
 
-<CodeGroup title="Adding an image">
 
 ```python {{ title: 'Python' }}
 from fastpdf import ImageFile
 
 image_path="my-logo.png"
 image_data = ImageFile(format="png", uri="my_favourite_logo")
 template_id = template["id"]
 res = client.add_image(template_id, image_path, image_data)
 ```
 
-</CodeGroup>
 
 Finally, we render our document. As usual, we define our rendering data object with our variable. 
 
-<CodeGroup title="Rendering our image template">
 
 ```python {{ title: 'Python' }}
+from fastpdf import ImageFile
+
+image_path="my-logo.png"
+image_data = ImageFile(format="png", uri="my_favourite_logo")
+
 template_id = template["id"]
-document_data = { 'name': "Jane" }
-document = client.render_template(template_id, document_data)
-client.save(document, "path/to/image-document.pdf")
+res = client.add_image(template_id, image_path, image_data)
 ```
 
-</CodeGroup>
 
 ## Custom Header and Footer
 
 By default, FastPDF will include a header, composed of the document title and the date, and a footer with page numbers. 
-You can turn them on and off separately when adding your [Template](templates#template) or during rendering with the 
-[RenderOptions](render#render-options).
+You can turn them on and off separately when adding your [Template](https://docs.fastpdfservice.com/templates#template) or during rendering with the 
+[RenderOptions](https://docs.fastpdfservice.com/render#render-options).
 
 It is also possible to add custom headers and footers to your PDF documents. These headers and footers can include images, and
 dynamic content such as the current page number, total number of pages, and the current date. Let's take a look at how to do this.
 
 Firstly, let's create a new template:
 
-<CodeGroup title="A simple template">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <h1>{{title}}</h1>
     <p>{{content}}</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="customer-header-footer-document", format="html")
 ```
 
-</CodeGroup>
 
 You might have noticed that we have not added the template yet. It is because we need to define our header and footer first.
-Headers and footers comes with [special HTML classes](templates#header-and-footer) that can be used to inject printing values into them.
+Headers and footers comes with [special HTML classes](https://docs.fastpdfservice.comtemplates#header-and-footer) that can be used to inject printing values into them.
 We will use them to set the page number.
 
 
-<CodeGroup title="Custom header and footer">
-
 ```python {{ title: 'Python' }}
 header_content = """
 <div style="text-align: center; padding: 10px; font-size: 8px;">
     <h2>{{header_note}}</h2>
 </div>
 """.encode()
 footer_content = """
@@ -337,105 +292,94 @@
 </div>
 """.encode()
 template = client.add_template(template_content, template_data, 
                                header_data=header_content, 
                                footer_data=footer_content)
 ```
 
-</CodeGroup>
 
 Now, when you render the PDF, pass the `header_note`, `title` and `content` in your data:
 
-<CodeGroup title="Rendering custom header document">
 
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 
     'title': "My document",  
     'content': "My document content",  
     'header_note': "This is my favorite header",  
 }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
+# Save to disk, if needed
 client.save(document, "path/to/custom-header-document.pdf")
 ```
 
-</CodeGroup>
 
 
 ## Generating Multiple PDFs
 
 The FastPDF API also provides the ability to generate multiple PDFs in a single API call. This feature, referred to as batch processing, can be useful in situations where you need to generate many PDFs with different data.
 
 The way batch processing works in FastPDF is that you provide an array of data objects, each of which corresponds to one PDF. Let's see how to do this in practice.
 
 First, let's prepare our template and data. Suppose we want to generate PDFs for each user in our system.
 
-<CodeGroup title="Basic template">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <h1>Welcome, {{name}}!</h1>
     <p>Email: {{email}}</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="image-document", format="html")
 template= client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 Here, the template contains placeholders for user data (name and email). Next, we will prepare our data array.
 Each element of the array corresponds to one document. Here we will render 3 documents.
 
-<CodeGroup title="List of data">
 
 ```python {{ title: 'Python' }}
 users = [
     {"name": "John Doe", "email": "john@example.com"},
     {"name": "Jane Doe", "email": "jane@example.com"},
     {"name": "Richard Roe", "email": "richie@example.com"},
 ]
 ```
 
-</CodeGroup>
 
 Finally, we can call the `render_template_many()` method with our template id and batch data.
 
-<CodeGroup title="List of data">
 
 ```python {{ title: 'Python' }}
 template_id = template["id"]
 zip_result = client.render_template_many(template_id, users)
 ```
 
-</CodeGroup>
 
 The `render_template_many()` method will return a zip file that contains the 3 PDFs. 
 You now have the choice between extracting the zip_result into a python list, or in a directory on your disk, both using the `extract()` method.
 
-<CodeGroup title="Extracting result PDFs">
 
 ```python {{ title: 'Python' }}
 # Save pdfs to the disk
 client.extract(zip_result, "path/to/directory/")
 
 # Or get a list of PDF
 pdfs = client.extract(zip_result)
 ```
-</CodeGroup>
 
 
 
 ## Support
 
 For any questions or support, reach out to us at `support@fastpdfservice.com`.
 
 ## License
 
 fastpdf Python Package is licensed under the MIT license. See LICENSE for more details.
 
 
-
-
```

### Comparing `fastpdf-1.0.0/README.md` & `fastpdf-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: fastpdf
+Version: 1.0.1
+Summary: SDK for PDF rendering, generation & transformation via Fast PDF Service.
+Home-page: https://github.com/fastpdfservices/fastpdf-python
+Author: Korian
+Author-email: korian@fastpdfservice.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
 # FastPDF Python Package
 
 Welcome to **fastpdf** Python Package, the versatile and quick solution for your PDF rendering needs. This package is a SDK for fastpdfservice.com REST API.
 
 ## Overview
 
 `fastpdf` is a Python package designed to simplify the PDF generation process. It streamlines the procedure of rendering HTML/CSS templates into a PDF document, offering granular control over the rendering options, and provides the ability to add images and barcodes into your PDFs.
@@ -33,85 +50,74 @@
 from fastpdf import PDFClient
 ```
 
 To start with, make sure you have your FastPDF service API token handy. 
 This is required for all API calls to the FastPDF service. You can find your token under API settings in 
 your [FastPDF profile](https://fastpdfservice.com/profile/api).
 
-<CodeGroup title="Register your token">
 
 ```python {{ title: 'Python' }}
 client = PDFClient("API_KEY")
 ```
 
-</CodeGroup>
-
-
 Please refer to the [documentation](https://docs.fastpdfservice.com) for more details on the available features.
 
 
 ## Creating a Basic Template
 
 Creating a basic template is simple. Let's start by creating an HTML document with a placeholder for a `name` variable.
-Then, you'll need to create a [Template](templates#template) object and set `name` and `format`.
-
+Then, you'll need to create a [Template](https://docs.fastpdfservice.com/templates#template) object and set `name` and `format`.
 
-<CodeGroup title="Creating a basic template">
 
 ```python {{ title: 'Python' }}
 from fastpdf import Template
 
 template_str = "<html><body>Hello world, my name is {{name}}!</body></html>".encode()
 template_data = Template(name="basic-document", format="html")
 template = client.add_template(template_str, template_data)
 ```
 
-</CodeGroup>
 
 <Note>
-  Make sure you do not forget to `encode()` your string. Otherwise, the string will be interpreted as a filename.
+  *Make sure you do not forget to `encode()` your string. Otherwise, the string will be interpreted as a filename.*
 </Note>
 
 In this template, `{{name}}` is a placeholder that will be replaced by a real value when generating a PDF. 
 
 ## Your First Rendering
 
 Now, let's bring our document to life. We've got our template id handy, and our data ready to be cast into the chosen template. 
 But don't worry if you've misplaced the template id - a quick detour to your [template dashboard](https://fastpdfservice.com/services/templates) will point you right to it.
 In our data object, we set a value for the `name` variable that we defined in our template.
 
-<CodeGroup title="Rendering our basic template">
 
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 'name': 'John' }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
 ```
 
-</CodeGroup>
 
 Finally, we save it to the disk using the `save()` convenience function.
 
-<CodeGroup title="Saving our document to the disk">
 
 ```python {{ title: 'Python' }}
 client.save(document, "path/to/basic-document.pdf")
 ```
 
-</CodeGroup>
 
 And that's it! You've just brought your first PDF to life.
 
 
 ## For Loops
 
 FastPDF allows for more complex templates. For instance, you can use control structures like for loops and if statements in your templates.
 Here is how to iterate over a list of items, using a for loop.
 
-<CodeGroup title="For Loop">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <ul>
     {% for item in items %}
@@ -121,38 +127,34 @@
 </body>
 </html>
 """.encode()
 template_data = Template(name="for-loop-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 In this template, `{% for item in items %}` starts the loop, and `{% endfor %}` ends it.
 
 Next, we define our rendering_data by associating a list of item value to the `items` key, and render our document.
 
-<CodeGroup title="Rendering our For Loop template">
-
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 'items': ["First item", "Second item", "Last item"] }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
+# Save to disk, if needed
 client.save(document, "path/to/loop-document.pdf")
 ```
 
-</CodeGroup>
 
 
 ## If Statements
 
 If statements can be used to conditionally include parts of the template, based on the rendering data. Here's an example:
 
-<CodeGroup title="If statement">
-
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     {% if user_premium %}
         <p>Welcome, premium user!</p>
     {% else %}
@@ -161,34 +163,32 @@
 </body>
 </html>
 """.encode()
 template_data = Template(name="if-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 In this example, `{% if user_premium %}` starts the if statement, and `{% endif %}` ends it. 
 If `user_premium` is true, the "Welcome, premium user!" message will be included in the generated PDF. 
 Otherwise, the "Welcome, regular user!" message will be included.
 
 ## Stylesheets
 
 <Note>
-    Please ensure that your stylesheets are written purely in CSS. As of now, FastPDF does not support precompiled CSS languages 
+    *Please ensure that your stylesheets are written purely in CSS. As of now, FastPDF does not support precompiled CSS languages 
     like SCSS, or CSS frameworks like Tailwind. 
-    Stick to standard CSS to ensure compatibility and successful rendering.
+    Stick to standard CSS to ensure compatibility and successful rendering.*
 </Note>
 
 You can do this in one of two ways: by using a separate stylesheet, or by using inline CSS. 
 
 The latter works as usual, by either
 setting the `style` property html tags, or by writing your css classes in the header of the template:
 
-<CodeGroup title="A template with style">
 
 ```html {{ title: 'HTML' }}
 <html>
 <head>
     my-class {
         color: #f43f54;
         font-size: 12px;
@@ -198,120 +198,109 @@
 <body>
     <p class='my-class'>Welcome, {{name}}!</p>
     <p style='color: #ccc'> Goodbye ! </p>
 </body>
 </html>
 ```
 
-</CodeGroup>
-
 Alternatively, you can use the `add_stylesheet()` method to add a stylesheet to your template:
 
-<CodeGroup title="A template with style">
 
 ```python {{ title: 'Python' }}
 from fastpdf import StylesheetFile
 
 stylesheet_path = "styles.css"
 stylesheet_data = StylesheetFile(format="css")
+
 template_id = template["id"]
 client.add_stylesheet(template_id, stylesheet_path, stylesheet_data)
-
 ```
 
-</CodeGroup>
 
 Your template will now be rendered with style !
 
 ## Adding an image
 
 FastPDF allows you to add images to your templates, which can then be rendered into your final PDF documents. Here's how you can accomplish this.
 
 To begin, we create our template with an `<img>` tag, using our image uri in the `src` property as followed:
 
-<CodeGroup title="Creating a template with an image">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <img src="{{my_favourite_logo}}">
     <p>Welcome, {{name}}!</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="image-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 Then, we add an image to our template, and set the same image uri. 
 This step can be done from your [template dashboard](https://fastpdfservice.com/services/templates).
 
-<CodeGroup title="Adding an image">
 
 ```python {{ title: 'Python' }}
 from fastpdf import ImageFile
 
 image_path="my-logo.png"
 image_data = ImageFile(format="png", uri="my_favourite_logo")
 template_id = template["id"]
 res = client.add_image(template_id, image_path, image_data)
 ```
 
-</CodeGroup>
 
 Finally, we render our document. As usual, we define our rendering data object with our variable. 
 
-<CodeGroup title="Rendering our image template">
 
 ```python {{ title: 'Python' }}
+from fastpdf import ImageFile
+
+image_path="my-logo.png"
+image_data = ImageFile(format="png", uri="my_favourite_logo")
+
 template_id = template["id"]
-document_data = { 'name': "Jane" }
-document = client.render_template(template_id, document_data)
-client.save(document, "path/to/image-document.pdf")
+res = client.add_image(template_id, image_path, image_data)
 ```
 
-</CodeGroup>
 
 ## Custom Header and Footer
 
 By default, FastPDF will include a header, composed of the document title and the date, and a footer with page numbers. 
-You can turn them on and off separately when adding your [Template](templates#template) or during rendering with the 
-[RenderOptions](render#render-options).
+You can turn them on and off separately when adding your [Template](https://docs.fastpdfservice.com/templates#template) or during rendering with the 
+[RenderOptions](https://docs.fastpdfservice.com/render#render-options).
 
 It is also possible to add custom headers and footers to your PDF documents. These headers and footers can include images, and
 dynamic content such as the current page number, total number of pages, and the current date. Let's take a look at how to do this.
 
 Firstly, let's create a new template:
 
-<CodeGroup title="A simple template">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <h1>{{title}}</h1>
     <p>{{content}}</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="customer-header-footer-document", format="html")
 ```
 
-</CodeGroup>
 
 You might have noticed that we have not added the template yet. It is because we need to define our header and footer first.
-Headers and footers comes with [special HTML classes](templates#header-and-footer) that can be used to inject printing values into them.
+Headers and footers comes with [special HTML classes](https://docs.fastpdfservice.comtemplates#header-and-footer) that can be used to inject printing values into them.
 We will use them to set the page number.
 
 
-<CodeGroup title="Custom header and footer">
-
 ```python {{ title: 'Python' }}
 header_content = """
 <div style="text-align: center; padding: 10px; font-size: 8px;">
     <h2>{{header_note}}</h2>
 </div>
 """.encode()
 footer_content = """
@@ -320,103 +309,96 @@
 </div>
 """.encode()
 template = client.add_template(template_content, template_data, 
                                header_data=header_content, 
                                footer_data=footer_content)
 ```
 
-</CodeGroup>
 
 Now, when you render the PDF, pass the `header_note`, `title` and `content` in your data:
 
-<CodeGroup title="Rendering custom header document">
 
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 
     'title': "My document",  
     'content': "My document content",  
     'header_note': "This is my favorite header",  
 }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
+# Save to disk, if needed
 client.save(document, "path/to/custom-header-document.pdf")
 ```
 
-</CodeGroup>
 
 
 ## Generating Multiple PDFs
 
 The FastPDF API also provides the ability to generate multiple PDFs in a single API call. This feature, referred to as batch processing, can be useful in situations where you need to generate many PDFs with different data.
 
 The way batch processing works in FastPDF is that you provide an array of data objects, each of which corresponds to one PDF. Let's see how to do this in practice.
 
 First, let's prepare our template and data. Suppose we want to generate PDFs for each user in our system.
 
-<CodeGroup title="Basic template">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <h1>Welcome, {{name}}!</h1>
     <p>Email: {{email}}</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="image-document", format="html")
 template= client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 Here, the template contains placeholders for user data (name and email). Next, we will prepare our data array.
 Each element of the array corresponds to one document. Here we will render 3 documents.
 
-<CodeGroup title="List of data">
 
 ```python {{ title: 'Python' }}
 users = [
     {"name": "John Doe", "email": "john@example.com"},
     {"name": "Jane Doe", "email": "jane@example.com"},
     {"name": "Richard Roe", "email": "richie@example.com"},
 ]
 ```
 
-</CodeGroup>
 
 Finally, we can call the `render_template_many()` method with our template id and batch data.
 
-<CodeGroup title="List of data">
 
 ```python {{ title: 'Python' }}
 template_id = template["id"]
 zip_result = client.render_template_many(template_id, users)
 ```
 
-</CodeGroup>
 
 The `render_template_many()` method will return a zip file that contains the 3 PDFs. 
 You now have the choice between extracting the zip_result into a python list, or in a directory on your disk, both using the `extract()` method.
 
-<CodeGroup title="Extracting result PDFs">
 
 ```python {{ title: 'Python' }}
 # Save pdfs to the disk
 client.extract(zip_result, "path/to/directory/")
 
 # Or get a list of PDF
 pdfs = client.extract(zip_result)
 ```
-</CodeGroup>
 
 
 
 ## Support
 
 For any questions or support, reach out to us at `support@fastpdfservice.com`.
 
 ## License
 
 fastpdf Python Package is licensed under the MIT license. See LICENSE for more details.
 
 
+
+
```

### Comparing `fastpdf-1.0.0/fastpdf/api.py` & `fastpdf-1.0.1/fastpdf/api.py`

 * *Files identical despite different names*

### Comparing `fastpdf-1.0.0/fastpdf/exceptions.py` & `fastpdf-1.0.1/fastpdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastpdf-1.0.0/fastpdf/models.py` & `fastpdf-1.0.1/fastpdf/models.py`

 * *Files identical despite different names*

### Comparing `fastpdf-1.0.0/fastpdf.egg-info/PKG-INFO` & `fastpdf-1.0.1/fastpdf.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpdf
-Version: 1.0.0
+Version: 1.0.1
 Summary: SDK for PDF rendering, generation & transformation via Fast PDF Service.
 Home-page: https://github.com/fastpdfservices/fastpdf-python
 Author: Korian
 Author-email: korian@fastpdfservice.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -50,85 +50,74 @@
 from fastpdf import PDFClient
 ```
 
 To start with, make sure you have your FastPDF service API token handy. 
 This is required for all API calls to the FastPDF service. You can find your token under API settings in 
 your [FastPDF profile](https://fastpdfservice.com/profile/api).
 
-<CodeGroup title="Register your token">
 
 ```python {{ title: 'Python' }}
 client = PDFClient("API_KEY")
 ```
 
-</CodeGroup>
-
-
 Please refer to the [documentation](https://docs.fastpdfservice.com) for more details on the available features.
 
 
 ## Creating a Basic Template
 
 Creating a basic template is simple. Let's start by creating an HTML document with a placeholder for a `name` variable.
-Then, you'll need to create a [Template](templates#template) object and set `name` and `format`.
+Then, you'll need to create a [Template](https://docs.fastpdfservice.com/templates#template) object and set `name` and `format`.
 
 
-<CodeGroup title="Creating a basic template">
-
 ```python {{ title: 'Python' }}
 from fastpdf import Template
 
 template_str = "<html><body>Hello world, my name is {{name}}!</body></html>".encode()
 template_data = Template(name="basic-document", format="html")
 template = client.add_template(template_str, template_data)
 ```
 
-</CodeGroup>
 
 <Note>
-  Make sure you do not forget to `encode()` your string. Otherwise, the string will be interpreted as a filename.
+  *Make sure you do not forget to `encode()` your string. Otherwise, the string will be interpreted as a filename.*
 </Note>
 
 In this template, `{{name}}` is a placeholder that will be replaced by a real value when generating a PDF. 
 
 ## Your First Rendering
 
 Now, let's bring our document to life. We've got our template id handy, and our data ready to be cast into the chosen template. 
 But don't worry if you've misplaced the template id - a quick detour to your [template dashboard](https://fastpdfservice.com/services/templates) will point you right to it.
 In our data object, we set a value for the `name` variable that we defined in our template.
 
-<CodeGroup title="Rendering our basic template">
 
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 'name': 'John' }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
 ```
 
-</CodeGroup>
 
 Finally, we save it to the disk using the `save()` convenience function.
 
-<CodeGroup title="Saving our document to the disk">
 
 ```python {{ title: 'Python' }}
 client.save(document, "path/to/basic-document.pdf")
 ```
 
-</CodeGroup>
 
 And that's it! You've just brought your first PDF to life.
 
 
 ## For Loops
 
 FastPDF allows for more complex templates. For instance, you can use control structures like for loops and if statements in your templates.
 Here is how to iterate over a list of items, using a for loop.
 
-<CodeGroup title="For Loop">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <ul>
     {% for item in items %}
@@ -138,38 +127,34 @@
 </body>
 </html>
 """.encode()
 template_data = Template(name="for-loop-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 In this template, `{% for item in items %}` starts the loop, and `{% endfor %}` ends it.
 
 Next, we define our rendering_data by associating a list of item value to the `items` key, and render our document.
 
-<CodeGroup title="Rendering our For Loop template">
-
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 'items': ["First item", "Second item", "Last item"] }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
+# Save to disk, if needed
 client.save(document, "path/to/loop-document.pdf")
 ```
 
-</CodeGroup>
 
 
 ## If Statements
 
 If statements can be used to conditionally include parts of the template, based on the rendering data. Here's an example:
 
-<CodeGroup title="If statement">
-
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     {% if user_premium %}
         <p>Welcome, premium user!</p>
     {% else %}
@@ -178,34 +163,32 @@
 </body>
 </html>
 """.encode()
 template_data = Template(name="if-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 In this example, `{% if user_premium %}` starts the if statement, and `{% endif %}` ends it. 
 If `user_premium` is true, the "Welcome, premium user!" message will be included in the generated PDF. 
 Otherwise, the "Welcome, regular user!" message will be included.
 
 ## Stylesheets
 
 <Note>
-    Please ensure that your stylesheets are written purely in CSS. As of now, FastPDF does not support precompiled CSS languages 
+    *Please ensure that your stylesheets are written purely in CSS. As of now, FastPDF does not support precompiled CSS languages 
     like SCSS, or CSS frameworks like Tailwind. 
-    Stick to standard CSS to ensure compatibility and successful rendering.
+    Stick to standard CSS to ensure compatibility and successful rendering.*
 </Note>
 
 You can do this in one of two ways: by using a separate stylesheet, or by using inline CSS. 
 
 The latter works as usual, by either
 setting the `style` property html tags, or by writing your css classes in the header of the template:
 
-<CodeGroup title="A template with style">
 
 ```html {{ title: 'HTML' }}
 <html>
 <head>
     my-class {
         color: #f43f54;
         font-size: 12px;
@@ -215,120 +198,109 @@
 <body>
     <p class='my-class'>Welcome, {{name}}!</p>
     <p style='color: #ccc'> Goodbye ! </p>
 </body>
 </html>
 ```
 
-</CodeGroup>
-
 Alternatively, you can use the `add_stylesheet()` method to add a stylesheet to your template:
 
-<CodeGroup title="A template with style">
 
 ```python {{ title: 'Python' }}
 from fastpdf import StylesheetFile
 
 stylesheet_path = "styles.css"
 stylesheet_data = StylesheetFile(format="css")
+
 template_id = template["id"]
 client.add_stylesheet(template_id, stylesheet_path, stylesheet_data)
-
 ```
 
-</CodeGroup>
 
 Your template will now be rendered with style !
 
 ## Adding an image
 
 FastPDF allows you to add images to your templates, which can then be rendered into your final PDF documents. Here's how you can accomplish this.
 
 To begin, we create our template with an `<img>` tag, using our image uri in the `src` property as followed:
 
-<CodeGroup title="Creating a template with an image">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <img src="{{my_favourite_logo}}">
     <p>Welcome, {{name}}!</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="image-document", format="html")
 template = client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 Then, we add an image to our template, and set the same image uri. 
 This step can be done from your [template dashboard](https://fastpdfservice.com/services/templates).
 
-<CodeGroup title="Adding an image">
 
 ```python {{ title: 'Python' }}
 from fastpdf import ImageFile
 
 image_path="my-logo.png"
 image_data = ImageFile(format="png", uri="my_favourite_logo")
 template_id = template["id"]
 res = client.add_image(template_id, image_path, image_data)
 ```
 
-</CodeGroup>
 
 Finally, we render our document. As usual, we define our rendering data object with our variable. 
 
-<CodeGroup title="Rendering our image template">
 
 ```python {{ title: 'Python' }}
+from fastpdf import ImageFile
+
+image_path="my-logo.png"
+image_data = ImageFile(format="png", uri="my_favourite_logo")
+
 template_id = template["id"]
-document_data = { 'name': "Jane" }
-document = client.render_template(template_id, document_data)
-client.save(document, "path/to/image-document.pdf")
+res = client.add_image(template_id, image_path, image_data)
 ```
 
-</CodeGroup>
 
 ## Custom Header and Footer
 
 By default, FastPDF will include a header, composed of the document title and the date, and a footer with page numbers. 
-You can turn them on and off separately when adding your [Template](templates#template) or during rendering with the 
-[RenderOptions](render#render-options).
+You can turn them on and off separately when adding your [Template](https://docs.fastpdfservice.com/templates#template) or during rendering with the 
+[RenderOptions](https://docs.fastpdfservice.com/render#render-options).
 
 It is also possible to add custom headers and footers to your PDF documents. These headers and footers can include images, and
 dynamic content such as the current page number, total number of pages, and the current date. Let's take a look at how to do this.
 
 Firstly, let's create a new template:
 
-<CodeGroup title="A simple template">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <h1>{{title}}</h1>
     <p>{{content}}</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="customer-header-footer-document", format="html")
 ```
 
-</CodeGroup>
 
 You might have noticed that we have not added the template yet. It is because we need to define our header and footer first.
-Headers and footers comes with [special HTML classes](templates#header-and-footer) that can be used to inject printing values into them.
+Headers and footers comes with [special HTML classes](https://docs.fastpdfservice.comtemplates#header-and-footer) that can be used to inject printing values into them.
 We will use them to set the page number.
 
 
-<CodeGroup title="Custom header and footer">
-
 ```python {{ title: 'Python' }}
 header_content = """
 <div style="text-align: center; padding: 10px; font-size: 8px;">
     <h2>{{header_note}}</h2>
 </div>
 """.encode()
 footer_content = """
@@ -337,98 +309,89 @@
 </div>
 """.encode()
 template = client.add_template(template_content, template_data, 
                                header_data=header_content, 
                                footer_data=footer_content)
 ```
 
-</CodeGroup>
 
 Now, when you render the PDF, pass the `header_note`, `title` and `content` in your data:
 
-<CodeGroup title="Rendering custom header document">
 
 ```python {{ title: 'Python' }}
-template_id = template["id"]
 document_data = { 
     'title': "My document",  
     'content': "My document content",  
     'header_note': "This is my favorite header",  
 }
+
+template_id = template["id"]
 document = client.render_template(template_id, document_data)
+# Save to disk, if needed
 client.save(document, "path/to/custom-header-document.pdf")
 ```
 
-</CodeGroup>
 
 
 ## Generating Multiple PDFs
 
 The FastPDF API also provides the ability to generate multiple PDFs in a single API call. This feature, referred to as batch processing, can be useful in situations where you need to generate many PDFs with different data.
 
 The way batch processing works in FastPDF is that you provide an array of data objects, each of which corresponds to one PDF. Let's see how to do this in practice.
 
 First, let's prepare our template and data. Suppose we want to generate PDFs for each user in our system.
 
-<CodeGroup title="Basic template">
 
 ```python {{ title: 'Python' }}
 template_content = """
 <html>
 <body>
     <h1>Welcome, {{name}}!</h1>
     <p>Email: {{email}}</p>
 </body>
 </html>
 """.encode()
 template_data = Template(name="image-document", format="html")
 template= client.add_template(template_content, template_data)
 ```
 
-</CodeGroup>
 
 Here, the template contains placeholders for user data (name and email). Next, we will prepare our data array.
 Each element of the array corresponds to one document. Here we will render 3 documents.
 
-<CodeGroup title="List of data">
 
 ```python {{ title: 'Python' }}
 users = [
     {"name": "John Doe", "email": "john@example.com"},
     {"name": "Jane Doe", "email": "jane@example.com"},
     {"name": "Richard Roe", "email": "richie@example.com"},
 ]
 ```
 
-</CodeGroup>
 
 Finally, we can call the `render_template_many()` method with our template id and batch data.
 
-<CodeGroup title="List of data">
 
 ```python {{ title: 'Python' }}
 template_id = template["id"]
 zip_result = client.render_template_many(template_id, users)
 ```
 
-</CodeGroup>
 
 The `render_template_many()` method will return a zip file that contains the 3 PDFs. 
 You now have the choice between extracting the zip_result into a python list, or in a directory on your disk, both using the `extract()` method.
 
-<CodeGroup title="Extracting result PDFs">
 
 ```python {{ title: 'Python' }}
 # Save pdfs to the disk
 client.extract(zip_result, "path/to/directory/")
 
 # Or get a list of PDF
 pdfs = client.extract(zip_result)
 ```
-</CodeGroup>
 
 
 
 ## Support
 
 For any questions or support, reach out to us at `support@fastpdfservice.com`.
```

### Comparing `fastpdf-1.0.0/setup.py` & `fastpdf-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name='fastpdf',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/fastpdfservices/fastpdf-python',
     author='Korian',
     author_email='korian@fastpdfservice.com',
     description='SDK for PDF rendering, generation & transformation via Fast PDF Service.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
```

