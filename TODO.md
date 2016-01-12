* Inline the styles:
  * Remove the to-string conversion
  * Stringify the properties only, and add them as a `style` attribute to the
    HTML node
  * Psuedo elements
    * Stringify psuedo elements' properties _along with the selector_, then add as
      a `<style>` tag as a child node to the node being converted
    * If node being converted cannot have children, throw a warning about losing
      psuedo selectors
    * Alternatively; Keep the separately generated stylesheets
* Ability to extract multiple nested components
  * Ask user to add the appropriate `data-` attribute on the elements?