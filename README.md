# Pathivu Landing Web

A svelte program that is used to build the landing page for [Pathivu](https://github.com/pathivu/pathivu)



## What is the structure?
The web page is built on a structure that uses custom sections and each section uses multiple elements. 


### So how does it work?

All files are Svelte based and they can be imported into another svelte page to be used as elements. For example

`import ELementName from "./elements/ElementName.svelte"`

this helps you use the element in the svelte file as elements or even sections. Each element has it's own properties that can be passed to make sure that no specific customization is needed. For Example

`<ElementName propertName="PropertyValue" />`


## What custom elements can you use?

* ### ButtonHolder
    
    Create buttons with ease, For Example

    `<ButtonHolder buttonText="Try Now" backgroundColor="#1E2F3E" textColor="#00A8B0" buttonImage="./images/right-arrow.svg" action="https://dashboard.pathivu.io" />`

    [View Example](./imagesForReadme/ButtonHolder.png)

    ##### Properties you can pass
    
    1. buttonText
        ###### This is the text on the button.

    2. backgroundColor 
        ###### This is the background colour of the button

    3. textColor
        ###### This is the color of the text in the button

    4. buttonImage
        ###### If the button has an image next to the text then you can link it here, can be url or a local link to the image. If no image then leave this blank.
    
    5. action
        ###### You can create a link that should be open on the click of the button.

* ### Paragraph
    
    Create buttons with ease, For Example

    `<Paragraph content="We love the people who love us, come spread love <3" alignText="center" />`

    [View Example](./imagesForReadme/Paragraph.png)

    ##### Properties you can pass
    
    1. content
        ###### This is the text in the Paragraph

    2. alignText 
        ###### This can have multiple values link center, justified, left and right.   

* ### LargeHeading
    
    Create buttons with ease, For Example

    `<LargeHeading beforeMarkedValue="The only" markedValue="logging" afterMarkedValue="platform you need" alignText="left" />`

    [View Example](./imagesForReadme/LargeHeading.png)

    ##### Properties you can pass

    ###### Headings have a feature of changing colour of a certain part to highlight. 
    
    1. beforeMarkedValue
        ###### Anything before highlighted word comes here.

    2. markedValue
        ###### Your highlighted work or part is this.

    3. afterMarkedValue
        ###### Anything after the highlighted comes here.

    4. alignText 
        ###### This can have multiple values link center, justified, left and right. 

* ### InformationCard
    
    Create buttons with ease, For Example

    ` <InformationCard iconColor="#00A8B0" iconBackgroundColor="#1E2F3E" paragraphText="A couple of line about the feature will help the person understand better" headingText="Log tailing" imageURL="./images/log-tailing.svg" />`

    [View Example](./imagesForReadme/InformationCard.png)

    ##### Properties you can pass

    ###### Headings have a feature of changing colour of a certain part to highlight. 
    
    1. iconColor
        ###### This is the color of the icon and also the color of the heading.

    2. markedValue
        ###### This is the background color of the icon holder box.

    3. paragraphText
        ###### This is the content that comes under the heading of the card.

    4. headingText
        ###### This is the content that comes in the heading of the card.

    5. imageURL
        ###### This is the image that is inside the icon holder, or basically this is the icon. Link a web link or a local link.


## How does the compiling work?

Well it's fairly simple, clone the repository using the command

`git clone git@github.com:pathivu/pathivu-landing-web.git`

and cd into the repository folder

`cd pathivu-landing-web`

Now comes the svelte part, you start of with initialising all the files so that you can run the testing part.

`npm install`

Get started with development.


## How to test and deploy?

While developing just run, you will have auto refreshing sysetm deployed to localhost:5000

`npm run dev`

You can deploy on netlify by pointing to public folder and giving the command to run as npm run build.

Or if you want to take the local files to your server directly, just run

`npm run build`

and your files will be in the public folder, compiled.