BigCartel API
=============

PHP library interfacing the various functionality provided by Big Cartel's REST API


Store Information
-----------------

Usage:


	require('bigcartel.class.php');

	$BG = new BigCartel;
	$BG->setStore('labrecords');

	$store_info = $BG->getStoreInfo();

Refer to the [store documentation](http://help.bigcartel.com/customer/portal/articles/772750-variables#store) to review the various properties accessible in the response.


Products
--------

Listing all products:

	require('bigcartel.class.php');

	$BG = new BigCartel;
	$BG->setStore('labrecords');

	$products = $BG->listProducts();

Listing 5 products

	require('bigcartel.class.php');

	$BG = new BigCartel;
	$BG->setStore('labrecords');

	$products = $BG->listProducts(5);

Listing 5 products from category 'tees'

	require('bigcartel.class.php');

	$BG = new BigCartel;
	$BG->setStore('labrecords');

	$products = $BG->listProducts(5, 'tees');

Again, you can review details of the API response in their [products documentation](http://help.bigcartel.com/customer/portal/articles/772750-variables#product)