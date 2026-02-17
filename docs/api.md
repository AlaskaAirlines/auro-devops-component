# auro-slideshow

### Properties & Attributes

| Properties  | Attributes  | Type    | Default           | Description                                                                                                                                                                                         |
| ----------- | ----------- | ------- | ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| autoplay    | autoplay    | boolean | false             | If true, the slideshow will play automatically.                                                                                                                                                     |
| autoScroll  | autoScroll  | boolean | false             | If true, the slideshow will scroll continuously.                                                                                                                                                    |
| delay       | delay       | number  | 7000              | Slide duration in milliseconds. (Only used with `autoplay`)                                                                                                                                         |
| fullBleed   | fullBleed   | boolean | false             | If set, the slideshow will take up the width of its parent container showing previous and next slides. **Note:** a parent container must have `overflow-x: hidden` to prevent horizontal scrolling. |
| loop        | loop        | boolean | false             | If true, the slideshow will loop back to the first slide after reaching the last slide.                                                                                                             |
| navigation  | navigation  | boolean | false             | If true, the slideshow will display navigation arrows for previous and next slides when the slide container is hovered.                                                                             |
| pagination  | pagination  | boolean | false             | If true, the slideshow will display pagination dots for each slide. If autoplay is on, the active dot will also show a progress bar.                                                                |
| pauseLabel  | pauseLabel  | string  | "Pause slideshow" | The aria-label for the pause button.                                                                                                                                                                |
| playLabel   | playLabel   | string  | "Play slideshow"  | The aria-label for the play button.                                                                                                                                                                 |
| playOnInit  | playOnInit  | boolean | false             | If true, the slideshow will start playing automatically on page load when `autoplay` or `autoScroll` are on.                                                                                        |
| scrollSpeed | scrollSpeed | number  | 0.75              | Number of pixels auto scroll should advance per frame. (Only used with `autoScroll`)                                                                                                                |
| startDelay  | startDelay  | number  | 1000              | Delay in milliseconds before the auto scroll starts. (Only used with `autoScroll`)                                                                                                                  |

### Methods

| Name       | Parameters                                         | Return          | Description                                    |
| ---------- | -------------------------------------------------- | --------------- | ---------------------------------------------- |
| play       | None                                               | [object Object] | Starts the slideshow playback.                 |
| register   | `name` (string) - Custom element name to register. |                 | Registers the custom element with the browser. |
| scrollNext | None                                               | [object Object] | Scrolls to the next slide.                     |
| scrollPrev | None                                               | [object Object] | Scrolls to the previous slide.                 |
| stop       | None                                               | [object Object] | Stops the slideshow playback.                  |

### Slots

| Name      | Description                                                                 |
| --------- | --------------------------------------------------------------------------- |
| (default) | Default slot for the slides. Each child element will be treated as a slide. |

### CSS Shadow Parts

| Name              | Description                                 |
| ----------------- | ------------------------------------------- |
| next-button       | Use to style the next button control.       |
| play-pause-button | Use to style the play/pause button control. |
| prev-button       | Use to style the previous button control.   |