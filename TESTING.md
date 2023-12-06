# Testing Page Table of Contents

- [**During Development Testing**](#during-development-testing)
  - [**_Manual testing_**](#during-development-manual-testing)
  - [**_Bugs & fixes_**](#during-development-bugs-fixes)

## During Development Testing <a name="during-development-testing"></a>

During development i tested my project in various ways such as:

1. Manually testing each element's appearance and responsiveness using the chrome dev tools.
2. Used the peer-code-review channel on slack to get feedback from my fellow students and teachers.

### Manual Testing: <a name="during-development-manual-testing"></a>

- During testing i used 3 different browsers to ensure cross-compatibility such as:

  1. Google chrome
  2. Opera GX
  3. Bing

- I then used the dev tools on these browsers to test different screen sizes for for responsiveness.

## Bugs and Fixes <a name="during-development-bugs-fixes"></a>

1. Intended Outcome - For the nav section to stick to the top of the page and for it to shrink for different view-ports and also remain fixed to the top of the page when the user scroll's down.
   - Issue:
     - I was not able to stick the navigation to the top of the page without it being stuck to the left side of the page and not shrink to fit other view-ports.
   - Solution:
     - I wrapped the navigation inside a container which i applied display:flex and justify-content:center to and i applied max-width:1400px to the navigation itself.
2. Intended Outcome - For there to only be vertical scroll and no horizontal scroll on all view-ports.
   - Issue:
     - The images would overflow out of the view-port on small screen sizes and create horizontal scroll.
   - Solution:
     - I manually checked each image using the chrome dev tools to see which images overflowed out of the viewport and decreased their width to fit on smaller screen sizes.
3. Intended Outcome - For the owner details container in the eligibility form section to stick to the top of the page while the user scroll' down (on screen sizes larger than 998px).
   - Issue:
     - I did not have anything for the owner details div to stick to while the user was scrolling down.
   - Solution:
     - I added a div underneath the owners details div and gave it a width and height of 100% to fill in the open space, now when the owners details div is at the very top of the page and the user scrolls down, it overflows into the new div underneath, it also stops overflowing then the user scrolls past the entire section.
4. Intended Outcome - For when the user hovers over the logo, i wanted the paw icon next to it to rotate 45 degrees so it looks like the paw is waving.
   - Issue:
     - When i hovered over the logo, the entire logo rotated.
   - Solution:
     - I added the ":hover" pseudo code next to the logo like this ".logo:hover" and then after that i targeted the paw itself like this ".logo:hover .fa-paw"
