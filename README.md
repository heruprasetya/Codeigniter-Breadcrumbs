Breadcrumbs Library
18 October 2011

## Usage:

### Controller
```php
// This can be autoloaded //
$this->load->library('breadcrumbs');

// Assigning specific titles & links to specific parts of the path //
// as an array //
$this->breadcrumbs->page = array('link'=> base_url().'community' ,'title' => 'Community' );
$this->breadcrumbs->method = array('link'=> base_url().'community/people' ,'title' => 'People' );

// Variable passed into the view
$passed_to_view = $this->breadcrumbs->get();
```
### In your View
```html
<div class="path"><?php echo $breadcrumbs ?></div>
```
 
