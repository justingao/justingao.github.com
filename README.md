# Justin GAO' Blog on GitHub


## Howto Fork
If you want to fork this blog, please following these steps:

1. Make a new repository on [GitHub][github.com] named `USERNAME.github.com`, where **USERNAME** is your account on [GitHub][github.com].

2. Type the following commands to initialize the blog:

        git clone git@github.com:justingao/BlogTemplate.git USERNAME.github.com
        cd USERNAME.github.com
        git remote set-url origin git@github.com:USERNAME/USERNAME.github.com.git

3. Modify your personal settings in the `_config.yml` file, including: 

        #
        # Personal Info;
        #
        my:
            # Your name.
            name: Justin GAO
            # Your email.
            email: justin@leigao.org
            # GitHub Account.
            github: justingao
        
        #
        # Disqus settings.
        #
        disqus:
            # Disqus short name;
            shortname: justingao
        
        #
        # Google Analytics;
        #
        ga:
            # Google Analytics ID;
            id: UA-52005096-1
            # Google Analytics Site URL;
            uri: justingao.github.io

4. The site logo was stored in `media/image/logo.png`, you can replace it, which will be displayed in the `ABOUT` page.

5. OK, it time to write a new post for the blog site, all the posts were stored in `_post/` directory. The post filename should match the rule `YYYY-mm-dd-blog-title.md`, such as `2014-06-21-markdown-blog-example.md`.

6. After all, you can public your blog now.

        git add .
        git commit -a -m "First commit."
        git push origin master

You can access [https://USERNAME.github.io/](https://USERNAME.github.io/) to view your posts.


## Blog Structure
- \_config.yml

    Some basic settings, you should change the author and URL settings.

- \_posts

    Your blog posts.

- 404.md

    The ``Page Not Found'' page.

- links/index.md

    Exchange site's link here.

- google915045b4f6173450.html

    This file was generated from [Google Webmasters][google webmaster].


## Thanks

This blog is forked from [ellochen's blog](https://github.com/ellochen/ellochen.github.com)
Thanks for ellochen.



[github.com]:https://github.com/
[google webmaster]:https://www.google.com/webmasters/
