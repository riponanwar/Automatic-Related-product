# Automatic-Related-product

#This script populating 16 product. 
$this->_itemCollection =
        Mage::getResourceModel('catalog/product_collection')->addAttributeToSelect($attributes)
        ->addCategoryFilter($category)
        ->addStoreFilter()
        ->setPageSize(16) // display 16 related products
        ->setCurPage(1)
        ->addIdFilter(array($product_id), true);
