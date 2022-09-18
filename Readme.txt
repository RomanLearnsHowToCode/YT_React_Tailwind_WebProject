1_ fist commit

Tailwind Config Cjs
tailwind.config.cjs are copied from -> https://github.com/adrianhajdin/project_hoobank/blob/45b4958981ea82423693f6f31524ec8ef08651cb/tailwind.config.cjs
The changes contain colours, font and screen resolutions with breakpoints for mobile devices (responsive design)

Index.css
Index.css was also changed with -> https://github.com/adrianhajdin/project_hoobank/blob/45b4958981ea82423693f6f31524ec8ef08651cb/src/index.css 
These changes contain styles to be used with Tailwind

Constants -> index.js -> this will work with ASSETS as images and such and would create CONSTANTS from them, the constants are usefull for users,
they don't need to know how to code, just go there and do some changes.. easy / or add 

Style.js was copied from -> https://github.com/adrianhajdin/project_hoobank/blob/45b4958981ea82423693f6f31524ec8ef08651cb/src/style.js 
This style contain settings fro margins and flexes, layout, this is an important style to understand how aligning and positioning on website works like
collections of class names collected into name strings, so it is easier to use these

Creating components folder, react is all about components

Navbar function: 
${index === navLinks.length -1 ? 'mr-0' : 'mr-10'} - we are setting margin right 10 for each navLink entry, but it is the last entry in the list, then the margin will be 0


export default GetStarted


Spreading FEATURE properties, video time stamp - 1:20:53,  <FeatureCard key={feature.id} {...feature} index={index}  />
feature is an array of 4 values, id, icon, content, title, spreading the feature ... 

A great video to understand the positionining FINALLY of the items on web site, this might be a breakthrough for the portfolio website

Project completed, the big take over is the tailwind positioning and attributes.. nice and clean looking website.. 

- skipped deployment - https://youtu.be/_oO4Qi5aVZs