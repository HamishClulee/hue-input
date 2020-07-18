# hue-input

Timesaving component wrapping the &lt;input> element

This is not intended to be used as a dependency, feel free to copy paste, or use for reference though

Styled in a similar fashion to the Material Design inputs that animate the placeholder into the label position on focus

Provides a few props to quickly configure the input attributes; `hasautocomplete` `inptype` and `isrequired`

Emits a user defined event (defined via prop `eventname`) when the value of the input changes, this allows you to link your validation functions outside of the component

If the `inptype` prop is set to `password` the show / don't show icon will display, the value of input will be seen as a series of dots if 'don't show' is selected

The `errortxt` prop is implemented to allow users to display the result of their validation functions inside the component

I've found that this pattern is the quickest way to deal with multiple inputs on a page while maintaining as few validation functions as possible

It may be that providing another prop formatted as an array of functions which return a boolean would be a better way to approach validation, but it feels like over engineering at first glance
