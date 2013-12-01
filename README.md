<h1>jQuery Plugins</h1>
  <h3>Inline text editing plugin: jquery.inline.js</h3>
  <p></p>
  <h3>JSON to Form plugin: jquery.toForm.js</h3>
   <p></p>
  <h3>A simple form population plugin: jQuery.populate.js </h3>
</h1>

<h2>Documentation:</h2>

<h4>The inline plugin is a powerfull plugin used for making page text editable. The plugin takes an object; options parameter where textSize, defaultValue and a callback can be set.</h4>

[jquery Selector: html element].inline(options);

Example:

    $("#presentationTitle").inline({
        textSize: "250%",
        defaultValue: "Enter title of presentation here",
        callback: handlers.setTitle
    });


<h4>The toForm plugin appends a form into an html div from a JSON object</h4>


<h4>The populate plugin is bound to a jQuery/javascript selector; some form element and takes an object as a parameter.</h4> 

[jQuery Selector: Form].populate({key: value});

Example 1: 

            $("#myform").populate({
                name: "Frank C Prenell",
                title: "Complexities of modern theory",
                publication: "Bolthouse Publishing company",
                location: "New York"
            });

Example 2: 

            $("#slideForm").populate({
                title: slide.title,
                header: slide.header,
                content: slide.content,
                selectedTheme: app.presentations[index].selectedTheme
            });
