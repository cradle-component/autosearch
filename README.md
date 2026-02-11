# autosearch component
CradleCMS search web component.


## Installation
Put the `asearch.js` component in your themes `components` folder.

## How to use
Include the component and render the search field however you like inside the `<a-search>` tag. 
It listens on `input` and `keydown` events on the wrapped input text field. 

### search options
search options are passed in as attributes.

| attribute | example                      | meaning                             |
| --------- | ---------------------------- | ----------------------------------- |
| include   | products,pages,articles      | entities to include in the search   |
| filter    | title,id,handle              | filtered result fields              |
| delay     | 100                          | throttle delay in ms                |
| chars     | 3                            | min characters before searching     |
| limit     | 20                           | limit number of results             | 
| truncate  | 100                          | truncate search result titles       |

You can use more attributes as search query parameters, read more at [cradlecms.com](https://cradlecms.com/docs).


### Example
```
{% component 'asearch.js' %}
<a-search include="pages,articles,products" filter="title,image,featured_image,price,compare_at_price">
 <input type="search" placeholder="Search" />
</a-search>   
```

<img width="523" height="185" alt="search_web_component_example" src="https://github.com/user-attachments/assets/8d295fef-19b8-47e8-b2bc-a301b2ad8bc5" />
