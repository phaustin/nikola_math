* Master branch

  - Stock nikola repository created by ```nikola init``` followed by
    adding one line to conf.py to allow ipynb posts
    
    ```
    diff --git a/test/conf.py b/test/conf.py
    index c7e16d1..9010797 100644
    --- a/test/conf.py
    +++ b/test/conf.py
    @@ -169,7 +169,9 @@ THEME_COLOR = '#5670d4'
    POSTS = (
    ("posts/*.rst", "posts", "post.tmpl"),
    ("posts/*.txt", "posts", "post.tmpl"),
    +    ("posts/*.ipynb", "posts", "post.tmpl"),
    )
    +
    PAGES = (
     ("stories/*.rst", "stories", "story.tmpl"),
     ("stories/*.txt", "stories", "story.tmpl"),
   ```

   - The notebook posts/stock-delimiters.ipynb can't be converted
     to pdf. The html rendered notebook with the error message
     is at [stock-delimiters.html](https://htmlpreview.github.io/?https://github.com/phaustin/nikola_math/blob/master/test/posts/stock-delimiters.html)
     
