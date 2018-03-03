# FreeCodeCamp-CSS-Talk
## Lesson 01 Text Effects
    STAMPED LETTERING
        TEXT SHADOW
            right 1px down 2px blur 1 px color 10% brighter than the background color;
                text-shadow: 1px 2px 1px #8396a8;
        COLOR RGBA
            Black color with an opacity of .25
            color: rgba(0, 0, 0, 0.25);

    EMBOSSED LETTERING
        opacity: 0.3;
        Same color as background
            color: slategray;
        Shadow: Left 1 | Up 1 | Blur 1 | color white 
            comma for the next set of values
                Right 1 | Down 1 | Blur 1 | color black
                text-shadow: -1px -1px 1px #fff, 1px 1px 1px #000;
    3D Lettering
        Multiple Text Shadows for 3D lettering effect
            text-shadow: 0px 1px 0px #999,
                         0px 2px 0px #888, 0px 3px 0px #777, 
                         0px 4px 0px #666, 0px 5px 0px #555, 
                         0px 6px 0px #444, 0px 7px 0px #333, 
                         0px 8px 7px #001135;


## Lesson 02 Animated CSS Part 1
    Transform properties affects the appearance of an element on screen.
		translate: is a x y movement
		rotate: is a fixed point rotate (circular)
		scale: is a fixed point increase in size
		perspective: property determines the distance between the z=0 plane and the user in order to give a 3D-positioned element some perspective.

		translate: repositions an element in the horizontal and/or vertical directions. | translate(10px) (xy) or translate(10px, 20px) (x,y)
		translate3d: repositions an element in 3D space. | translate3d(42px, -62px, -135px); (x,y,z) 
		translateX: repositions an element horizontally on the 2D plane. | translateX(10px);
		translateY:  repositions an element vertically on the 2D plane. | translateY(10px);
		translateZ: repositions an element along the z-axis in 3D space (closer or further from the viewer starting at 0 | translateZ(42px);

		rotate3d: is a 3D space rotate | rotate3d(1, 1, 1, 45deg)
		rotatex: is a horizontal axis rotate | rotateX(45deg);
		rotatey: is a vertical axis rotate | rotateY(45deg);
		rotatez: is a z-axis rotate | rotateZ(90deg);

		scale: up down (x, y) or (both)
		scale3d: resizes an element in 3D space scale3d(x, y, z)
		scalex: resizes an element along the x-axis (horizontally) | scaleX(0.6);
		scaley: resizes an element along the y-axis (vertically) | scaley(0.6);
		scalez: resizes an element along the z-axis | scaleZ(0.6);
    ANIMATION PROPERTIES
        Find All Animatable Properties here
            https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties
        Animation is a css property that encompasses various animation properties
            animation-name
                Specifies one or more animations that should be applied to an element. Each name indicates an @keyframes at-rule that defines the property values for the animation sequence.
                    animation-name: nameOfAnimationKeyframes;

            animation-duration
                Specifies the length of time that an animation should take to complete one cycle.
                    /* Single animation */
                        animation-duration: 6s;
                        animation-duration: 120ms;
                    /* Multiple animations */
                        animation-duration: 1.64s, 15.22s;
                        animation-duration: 10s, 35s, 230ms;

            animation timing-function
                Specifies how a CSS animation should progress over the duration of each cycle.
                    animation-timing-function: ease;
                    animation-timing-function: ease-in;
                    animation-timing-function: ease-out;
                    animation-timing-function: ease-in-out;
                    animation-timing-function: linear;
                    animation-timing-function: step-start;
                    animation-timing-function: step-end;

            animation-delay
                Specifies when an animation should start
                    animation-delay: 3s;
                    animation-delay: 0s;

            animation-iteration-count
                Specifies the number of times an animation cycle should be played before stopping.
                    animation-iteration-count: infinite;
                    animation-iteration-count: 3;

                
            animation-direction
                Specifies whether an animation should play forwards, backwards, or alternating back and forth.
                    animation-direction: normal;
                    animation-direction: reverse;
                    animation-direction: alternate;
                    animation-direction: alternate-reverse;

            animation-fill-mode
                Specifies how a CSS animation should apply styles to its target before and after its execution.
                    None
                        No applied styles
                            animation-fill-mode: none;
                    Forwards
                        Target will retain the computed values set by the last keyframe encountered during execution set by the animation-direction and animation-iteration-count
                            animation-fill-mode: forwards;
                    Backwards
                        Target will retain the computed values set by the first keyframe encountered during execution set by the animation-direction and animation-iteration-count
                            animation-fill-mode: backwards;
                            animation-fill-mode: both;

            animation-play-state
                specifies whether an animation is running or paused. This can be controlled by javascript to pause or resume animation playback
                    animation-play-state: running;
                    animation-play-state: paused;

## Lesson 02 Animated CSS Part 2
    ADVANCED TRANSFORM ANIMATION
        Faking motion blur
            Text Shadow
                Animating Text Shadow for text motion blur
            Box Shadow
                Property is used to add shadow effects around an element's frame. You can specify multiple effects separated by commas if you wish to do so. A box shadow is described by X and Y offsets relative to the element, blur and spread radii, and color.
                    /* offset-x | offset-y | blur-radius | color */

## Lesson 03 3D Box
    3D Cube
        Perspective-origin 
            CSS property determines the position at which the viewer is looking. It is used as the vanishing point by the perspective property.	

        Perspective
            The perspective CSS property determines the distance between the z=0 plane and the user in order to give a 3D-positioned element some perspective.

        transform-style: preserve-3d
            Indicates that the children of the element should be positioned in the 3D-space.

        transform-origin
            The transformation origin is the point around which a transformation is applied. For example, the transformation origin of the rotate() function is the center of rotation. 
                    top
                    bottom
                    right
                    left
                    center
                    Pixels
