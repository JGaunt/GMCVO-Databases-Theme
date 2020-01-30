GMCVO Databases Porto subtheme

This theme provides templates that have pre-defined styling in order to provide reponsive blocks that require minimal editing. In order to get this theme to work properly you must attach the correct styles to the
corresponding block. You may need to use templates.gmcvodatabases.org.uk as a reference guide but below give an overview of each block and the class assigned along with other important information needed to make
the theme work easily.



********************************
********** MODULES *************
********************************

Firstly, these are the recommended modules to get started with the GMCVO Porto subtheme. To make it easier, you may zip the modules folder in templates.gmcvodatabases.org.uk and unpack this in the new website's
module folder. Some of these modules will already be installed in the core Drupal filesystem.

- admin_menu
- admin_menu_toolbar
- block
- block_class -> This is required to give blocks the classes that will pull the styling as appropriate
- ctools
- ckeditor
- color
- comment
- contextual
- dashboard
- dblog
- features
- field
- field_sql_storage
- field_ui
- file
- file_entitiy
- filter
- help
- image
- imce
- jquery_update
- libraries
- list
- media
- media_wysiwyg
- menu
- module_filter
- node
- number
- options
- path
- pathauto -> Recommended for getting URLs to be automatically generated
- porto_custom_content
- porto_views
- rdf
- search
- shortcut
- stylizer
- system
- taxonomy
- tb_megamenu
- text
- token -> Required for pathauto
- toolbar
- update
- user
- views
- views_ui
- webform



********************************
*********** BLOCKS *************
********************************

The blocks below have been seperated by the pages they appear on and then by block order to make it easy to see which blocks do what by using templates.gmcvodatabases.org.uk as a reference guide although the blocks
may be used in whichever order is preferable to the client provided they have the correct class.


Homepage 1: Banner Image with Centered Title, Text and CTA

	Help:
	This block features a large banner image taking up the full width of the screen with a portion cut out of the center bottom with space for a title, some text and a call to action button.
	Within the title, text and call to action, the image will appear in full on its own. 
	In the block, add a large image of your choosing, if the image is not big enough, it may appear pixelated. The image must go first in the block with the title, text and call to action in an order of your choice.
	Ensure the title is in a heading font, heading  1 works best.
	Everying after the image must be wrapped in a <div> with the class "text".
	
	Example:
	<img src="/sites/default/files/image.jpg"/>
	<div class="text">
		<h1>Title</h1>
		<p>Text</p>
		<a href="#">link</a>
	</div>


	Class:
	.homepage-1-block-1

	Region:
	Before Content


Homepage 1: Call to Action with Image

	Help:
	This block feature a heading with a subheading and a call to action box with a heading, text and link on one side and an image, with a heading link overlay. There are three <div> tags that make up this block. The 
	first for the header, one for the right side text with the class "text" and one with the class "image".

	Example:
	<div class="header">	
		<h1>Title</h1>
		<p>Subheading</p>
	</div>
	<div class="text">
		<h2>Heading</h2>
		<p>Text</p>
		<a href="#">Link</a>
	</div>
	<div class="image">
		<img src="/sites/default/files/image.jpg"/> 
		<a href="#">Link</a>
	</div>


	Class:
	.homepage-1-block-2

	Region: Content


Homepage 1: Two Call to Actions with Images

	Help:
	This block features two images with a heading and subheading underneath both. There are two tables that make up this block, one for either image and their respective headings. The tables help keep both sides seperate
	which enables for easy responsiveness. Each table should have 2 rows and 1 column. The image goes in the top row and the text in the bottom.

	Example:
	<table>
		<tbody>
			<tr>
				<td><img alt="" src="/sites/default/files/image.jpg" /></td>
			</tr>
			<tr>
				<td>
					<h3><a href="#">Nunc vulputate</a></h3>
					<p>Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.</p>
				</td>
			</tr>
		</tbody>
	</table>
	<table>
		<tbody>
			<tr>
				<td><img alt="" src="/sites/default/files/person-holding-clear-plastic-bottle-3480494.jpg" /></td>
			</tr>
			<tr>
				<td>
					<h3><a href="#">Pellentesque et lobortis</a></h3>
					<p>Curabitur venenatis nunc pellentesque nulla vestibulum posuere.</p>
				</td>
			</tr>
		</tbody>
	</table>

	Class: 
	.homepage-1-block-3

	Region:
	Content




News Page 1: Banner with featured content overlay

	Help: 
	This block is made up of a view. To get this to work, you will need a view of articles that has the fields Image, Title and the date posted. An image or video needs to be put into the header of the view. This
	block supports both an image as well as a video. Header supports <h1> tag for a title to the page. Uses the default Article content type. Block should have the class newspage-1-view-1. The view does not need a class.

	Class:
	.newspage-1-view-1

	Region:
	Content
	

Side Bar: Quick Links with gradient background

	Help: 
	This block is a simple list of links or text. Background image is determined in the CSS, the rainbow overlay will adjust to any image. Block title is styled. Very easy to implement. Only tested on right sidebar.

	Example:
	<p><a href="#">A link</a></p>
	<p><a href="#">Another link</a></p>
	<p><a href="#">Yes, it's a link</a></p>
	<p>Not a link</p>
	
	Class: 
	.sidebar-1

	Region:
	Right Sidebar


Buttons 1: Colorful buttons with background change on hover

	Help:
	Just a list of links in the block, nothing special. Block colors are set to repeat every 4 so you can add as many or as little as you want.

	Example:
	<p><a href="#">Button</a></p>
	<p><a href="#">Button</a></p>
	<p><a href="#">Button</a></p>
	<p><a href="#">Button</a></p>

	Class:
	.buttons-1

	Region:
	Content























