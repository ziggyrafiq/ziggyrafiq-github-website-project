# Ziggy Rafiq Github Website

## Requirments

An insight into ZiggyRafiq.com is required, including blog posts, demo projects, and skills. Since the GitHub Website is static, it demonstrates using HTML5, CSS3(SASS) and JavaScript to create a simple, responsive website with just HTML5, CSS3(SASS/SCSS) and JavaScript.

The purpose of this website is to showcase Ziggy Rafiq's overall profile as well as some of his blog posts and demo projects. Also, this project is licensed under the MIT license, so anyone interested in using it must contact Ziggy Rafiq before doing so and must include a link to https://ziggyrafiq.com, and anyone wanting to learn from it should include a link to https://ziggyrafiq.com.

## Solution

It consists of a clean, easy-to-navigate static website, which can be accessed via https://ziggyrafiq.github.io and dynamic data is loaded by JSON files, which are updated by Ziggy Rafiq Rest APIs.

### Project Folder Structure

For this project I have used a simple, generic website structure, which I normally create.

You Can find a template name Baseplate HTML5, which I have created as a starting point for designing and development a website/web application.

    |- Src/
    	 |- Data/
    		   |- projects.json
    		   |- blogs.json
    	 |- Images/
    			 |- ziggy-rafiq-og-twitter-banner.png
    			 |- ziggy-rafiq-photo.png
    			 |- zr-github-bg.png
    			 |- LH-Demo-Project-Exercise.png
    			 |- IS-Demo-Project-Exercise.png
    			 |- How-to-use-Enum-Data-Values-with-Dot-Net-6.0-Framework-and-Entity-Framework-Core-6.png
    			 |- How-to-be-a-successful-Software-Consultant-Full-Stack-Designer-and-Developer.png
    			 |- Agile-Scrum-Definitions.png
    			 |- 12-Principles-of-Agile-by-Ziggy-Rafiq.png
    	|- Scripts/
    			 |- _Blog-Posts.js
    			 |- _Demo-Projects.js
    			 |- _Tabs.js

    	|- Styles/
    		    |- CSS/
    				 |- ZR-Styles.min.css
    	|- Fonts/
        	   |- fa-brands-400.ttf
        	   |- fa-brands-400.woff2
        	   |- fa-regular-400.ttf
        	   |- fa-regular-400.woff2
        	   |- fa-solid-900.ttf
        	   |- fa-solid-900.woff2
        	   |- fa-v4compatibility.ttf
        	   |- fa-v4compatibility.woff2
        |- Icons/
    			| - FavIcon/
    					   |- android-icon-36x36.png
    					   |- android-icon-48x48.png
    					   |- android-icon-72x72.png
    					   |- android-icon-36x36.png
    					   |- android-icon-96x96.png
    					   |- android-icon-144x144.png
    					   |- android-icon-192x192.png
    					   |- apple-icon.png
    					   |- apple-icon-57x57.png
    					   |- apple-icon-72x72.png
    					   |- apple-icon-76x76.png
    					   |- apple-icon-114x114.png
    					   |- apple-icon-120x120.png
    					   |- apple-icon-144x144.png
    					   |- apple-icon-152x152.png
    					   |- apple-icon-180x180.png
    					   |- apple-icon-precomposed.png
    					   |- favicon.ico
    					   |- favicon-16x16.png
    					   |- favicon-32x32.png
    					   |- favicon-96x96.png
    					   |- ms-icon-70x70.png
    					   |- ms-icon-144x144.png
    					   |- ms-icon-150x150.png
    					   |- ms-icon-310x310.png
    					   |- amanifest.json
    					   |- browserconfig.xml
        |- SASS/
        	  |- Mixins/
        	          |- _Directory.scss
        	          |- _Media-Queries.scss
        	          |- _Pie-Chart.scss
        	          |- _Progress-Bar.scss
        	    |- Vendors/
        	             |- Bootstrap/
        	             			|- mixins/
    										|- _border-radius.scss
    										|- _box-shadow.scss
    										|- _breakpoints.scss
    										|- _buttons.scss
    										|- _clearfix.scss
    										|- _container.scss
    										|- _deprecate.scss
    										|- _gradients.scss
    										|- _grid.scss
    										|- _image.scss
    										|- _list-group.scss
    										|- _lists.scss
    										|- _resize.scss
    										|- _transition.scss
    										|- _utilities.scss
    								|- utilities/
    										|- _api.scss
    								|- vendor/
    										|- _rfs.scss
    								|- _bootstrap.scss
    								|- _buttons.scss
    								|- _card.scss
    								|- _containers.scss
    								|- _functions.scss
    								|- _grid.scss
    								|- _images.scss
    								|- _mixins.scss
    								|- _reboot.scss
    								|- _root.scss
    								|- _utilities.scss
    								|- _variables.scss
        	             |- Fontawesome/
    								|- scss/
    									  |- _brands.scss
    									  |- _core.scss
    									  |- _fontawesome.scss
    									  |- _functions.scss
    									  |- _icons.scss
    									  |- _mixins.scss
    									  |- _regular.scss
    									  |- _screen-reader.scss
    									  |- _sizing.scss
    									  |- _solid.scss
    									  |- _variables.scss
        	  |- _Directory.scss
        	  |- _Buttons.scss
        	  |- _Card.scss
        	  |- _Charts.scss
        	  |- _Helpers.scss
        	  |- _Page.scss
        	  |- _Tabs.scss
        	  |- _Typography.scss
        	  |- _Variables.scss
        	  |- _ZR-Styles.scss
    	|- index.html
    |- Dist/
    	  |- Data/
    			|- projects.json
    	  |- Images/
    			 |- ziggy-rafiq-og-twitter-banner.png
    			 |- ziggy-rafiq-photo.png
    			 |- zr-github-bg.png
    			 |- LH-Demo-Project-Exercise.png
    			 |- IS-Demo-Project-Exercise.png
    			 |- How-to-use-Enum-Data-Values-with-Dot-Net-6.0-Framework-and-Entity-Framework-Core-6.png
    			 |- How-to-be-a-successful-Software-Consultant-Full-Stack-Designer-and-Developer.png
    			 |- Agile-Scrum-Definitions.png
    			 |- 12-Principles-of-Agile-by-Ziggy-Rafiq.png
    	  |- Scripts/
    			|- ZR-Scripts.min.js
    	  |- Styles/
    			|- CSS/
    				 |- ZR-Styles.min.css
    	  |- Fonts/
    			|- fa-brands-400.ttf
    			|- fa-brands-400.woff2
    			|- fa-regular-400.ttf
    			|- fa-regular-400.woff2
    			|- fa-solid-900.ttf
    			|- fa-solid-900.woff2
    			|-fa-v4compatibility.ttf
    			|- fa-v4compatibility.woff2
    	  |- Icons/
    			|- FavIcon/
    	    			  |- android-icon-36x36.png
    	    			  |- android-icon-48x48.png
    	    			  |- android-icon-72x72.png
    	    			  |- android-icon-36x36.png
    	    			  |- android-icon-96x96.png
    	    			  |- android-icon-144x144.png
    	    			  |- android-icon-192x192.png
    	    			  |- apple-icon.png
    	    			  |- apple-icon-57x57.png
    	    			  |- apple-icon-72x72.png
    	    			  |- apple-icon-76x76.png
    	    			  |- apple-icon-114x114.png
    	    			  |- apple-icon-120x120.png
    	    			  |- apple-icon-144x144.png
    	    			  |- apple-icon-152x152.png
    	    			  |- apple-icon-180x180.png
    	    			  |- apple-icon-precomposed.png
    	    			  |- favicon.ico
    	    			  |- favicon-16x16.png
    	    			  |- favicon-32x32.png
    	    			  |- favicon-96x96.png
    	    			  |- ms-icon-70x70.png
    	    			  |- ms-icon-144x144.png
    	    			  |- ms-icon-150x150.png
    	    			  |- ms-icon-310x310.png
    	    			  |- amanifest.json
    	    			  |- browserconfig.xml

    |- index.html
    |- .vscode/
    |- launch.json
    |- gulpfile.js
    |- node_modules/
    |- package.json
    |- ReadMe.md
    |- ReadMe.Docx

## Tool Used
The tools I used to build my website Ziggy Rafiq GitHub version are Microsoft VS Code for coding and Adobe Photoshop for designing the UI and GUI of the website. Keeping everything simple and clean so that later a junior developer or even a senior develop can take this project and make use of it for their own use. Please note that when you do make this project use for your own project, please let me know and please do not remove any copyright comments.

## License

This project is licensed under the MIT license and is released under the MIT license (http://opensource.org/licenses/MIT) and can be used under the MIT license as you inform Ziggy Rafiq by emailing to (ziggy@ziggyrafiq.com) and you must include the LICENSE file in your project and the author of this project (Ziggy Rafiq | https://ziggyrafiq.com).
