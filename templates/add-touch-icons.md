Created by: Alex Hardy
Created date: 2015-09-28
Last updated: 2015-09-28
Authors: Alex Hardy
Title: How do I add touch icons to my site?
Tags: templates

# How do I add touch icons to my site?

## You want to add touch icons, without uploading multiple image files for each size

You can use Perch's [image resize features](https://grabaperch.com/features/upload-crop-and-resize-images) tag to do that. Create a Perch editable region, using the code below as a template. You'll want to make the region shared, and place it in the head of your pages.

	<!-- For Chrome for Android: -->
	<link rel="icon" sizes="192x192" href="<perch:content id="icon" type="image" label="Image" bucket="touch-icon" width="192" height="192" help="Upload a 200 pixels square image" />" />
	<!-- For iPhone 6 Plus with @3× display: -->
	<link rel="apple-touch-icon-precomposed" sizes="180x180" href="<perch:content id="icon" type="image" bucket="touch-icon" label="Image" width="180" height="180" help="Upload a 200 pixels square image" />" />
	<!-- For iPad with @2× display running iOS ≥ 7: -->
	<link rel="apple-touch-icon-precomposed" sizes="152x152" href="<perch:content id="icon" type="image" bucket="touch-icon" label="Image" width="152" height="152" help="Upload a 200 pixels square image" />" />
	<!-- For iPad with @2× display running iOS ≤ 6: -->
	<link rel="apple-touch-icon-precomposed" sizes="144x144" href="<perch:content id="icon" type="image" bucket="touch-icon" label="Image" width="144" height="144" help="Upload a 200 pixels square image" />" />
	<!-- For iPhone with @2× display running iOS ≥ 7: -->
	<link rel="apple-touch-icon-precomposed" sizes="120x120" href="<perch:content id="icon" type="image" bucket="touch-icon" label="Image" width="120" height="120" help="Upload a 200 pixels square image" />" />
	<!-- For iPhone with @2× display running iOS ≤ 6: -->
	<link rel="apple-touch-icon-precomposed" sizes="114x114" href="<perch:content id="icon" type="image" bucket="touch-icon" label="Image" width="114" height="114" help="Upload a 200 pixels square image" />" />
	<!-- For the iPad mini and the first- and second-generation iPad (@1× display) on iOS ≥ 7: -->
	<link rel="apple-touch-icon-precomposed" sizes="76x76" href="<perch:content id="icon" type="image" bucket="touch-icon" label="Image" width="76" height="76" help="Upload a 200 pixels square image" />" />
	<!-- For the iPad mini and the first- and second-generation iPad (@1× display) on iOS ≤ 6: -->
	<link rel="apple-touch-icon-precomposed" sizes="72x72" href="<perch:content id="icon" type="image" bucket="touch-icon" label="Image" width="72" height="72" help="Upload a 200 pixels square image" />" />
	<!-- For non-Retina iPhone, iPod Touch, and Android 2.1+ devices: -->
	<link rel="apple-touch-icon-precomposed" href="<perch:content id="icon" type="image" label="Image" bucket="touch-icon" width="57" height="57" help="Upload a 200 pixels square image" />" /><!-- 57×57px -->
	<perch:content type="image" id="icon" label="Image" bucket="touch-icon" width="200" height="200" suppress="true" help="Upload a 200 pixels square image" />