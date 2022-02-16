What is VC-Toggle-Switch?
===================================

This is a little toggle I made that is completely independent of framework. It is highly customizable, and will look good within any app.

Why?
===================================

I made this so I could use it inside an AngularJS (1.0.0) app, and I think your reasons should be the same: you're looking for something that will work anywhere, and that looks good.

How do I use this?
===================================

This toggle was made in a way that you won't need much (or any) CSS to adapt it into your app. It also should be very plug'n play. This is an easy example of its implementation:

    <div class="vc-toggle-container">
      <label class="vc-switch">
        <input type="checkbox" class="vc-switch-input" />
        <span class="vc-switch-label" data-on="Yes" data-off="No"></span>
        <span class="vc-handle"></span>
      </label>
    </div>

This is the basic structure that will generate the default toggle. Also, don't forget to import its CSS file into your HTML:

    <link rel="stylesheet" type="text/css" href="vc-toggle-switch.css" />

How do I change its visual?
===================================

That sould be very simple, here's an example of a customized toggle:

      <div 
        style="
          --vc-off-color: blue;
          --vc-on-color: blue;
          --vc-on-font-color: red;
          --vc-off-font-color: red;
        "
        class="text-center d-inline-block"
      >
        <div class="vc-toggle-container">
          <label class="vc-switch">
            <input type="checkbox" class="vc-switch-input" />
            <span 
              data-on="Yes" 
              data-off="No"
              class="vc-switch-label"
            ></span>
            <span class="vc-handle"></span>
          </label>
        </div>
      </div>

As you can see, all you have to do is add the CSS properties you want to change in the style of the outermost main div.

Which properties can I change?
===================================

- Background color when it's turned off

      --vc-off-color


- Background color when it's turned on

      --vc-on-color

  
- Animation speed and type

      --vc-animation-speed


- Font used by the text

      --vc-font-family


- The size used

      --vc-font-size


- The font weight

      --vc-font-weight

  
- Font color when the switch is on

      --vc-on-font-color


- Font color when the switch is off

      --vc-off-font-color


- How far the OFF text is from the right side

      --vc-label-position-off


- How far the ON text is from the left side

      --vc-label-position-on


- Small switch width

      --vc-width


- Small switch height

      --vc-height


- Border radius for the handle

      --vc-handle-border-radius


- Border radius for the box

      --vc-box-border-radius


- Shadow for the handle

      --vc-handle-shadow

  
- Handle color

      --vc-handle-color


- Handle width

      --vc-handle-width


- Handle height

      --vc-handle-height


- The handle's width while the toggle is clicked

      --vc-onclick-width


- Hadle's distance from the top

      --vc-handle-top


You can find every property being used in the `vc-toggle-switch.css` file.

Where can I see this in action?
===================================

If you want to take a look at some working examples, you can check it here: https://vc-toggle.stackblitz.io

And if you want to play with it a little bit, take a look here: https://stackblitz.com/edit/vc-toggle?file=index.html

Note: Stackblitz is a little funky, and I couldn't make it load the CSS as an import. I recommend you downloading the project and playing a bit on yout own machine.

That's all, folks!
===================================
Please, take a moment to connect with me on Linkedin: https://linkedin.com/in/vinicius-chab/, and have a great day!

License
===================================
MIT - Vinícius Chab
