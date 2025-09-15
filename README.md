* What design principles guided your improvements?
        
Gestalt’s Design Principles are well known in the designer community as they drive intuitiveness and ease out of the user. They 	are as follows:
   1. Proximity:
	Objects placed close together are perceived as a group. 
   2. Similarity:
	Elements that share similar attributes (like shape, color, or size) are grouped together. 
   3. Continuity:
	The eye naturally follows smooth paths and curves, preferring to see a continuous flow of elements. 
   4. Closure:
	The brain tends to fill in missing information to perceive incomplete shapes as whole, complete objects. 
   5. Figure/Ground:
	The human eye automatically separates a design into a main figure (the focal point) and the surrounding ground (the background). 
   6. Uniform Connectedness:
	Objects connected by visual elements (like lines or shapes) are perceived as a more related group.

I have tried my best to de-clutter the design and put forth the functionalities of the application.

* How did you ensure responsiveness across devices?

  
To ensure responsiveness, I used the Bootstrap framework, which provides:
   * Mobile-First Design: Optimized first for smaller screens, then scales up using media queries.

   * 12-Column Grid System: Allows flexible layout control across different screen sizes using classes like col-sm-*, col-md-*, etc.

   * Responsive Breakpoints: Predefined width-based breakpoints (sm, md, lg, xl) let styles adapt to various devices.

   * Viewport Meta Tag: Ensures proper rendering and touch zooming across all devices.


* What trade-offs did you make between the design and performance?


Trade-offs between design and performance:
To enhance the user experience, we incorporated rich UI elements like:
  * Background images

  * External libraries (e.g., Bootstrap, Flatpickr)

  * Custom styling and layout

  * Responsive images and icons

These improvements increase visual appeal and usability, but come with trade-offs:
* Performance Impact:

* Slightly slower initial load time due to external CSS/JS files and images

* Higher bandwidth usage on low-speed networks

* Mitigation:

* Used CDNs for faster library loading

* Kept custom CSS minimal and scoped

* Optimized images for web use

Overall, we prioritized accessibility and clarity of information while keeping performance degradation minimal and acceptable for a modern web environment.

* What was the most challenging part of the task and how did you approach it?

  
The biggest challenge was understanding and navigating an existing Django codebase (FOSSEE Workshop Booking System) that had limited documentation and used older Django syntax (e.g., url() instead of path()), which caused compatibility issues with newer Django versions.
How I approached it:
* Carefully traced the views, forms, and models to understand the workflow.

* Resolved missing database tables by identifying and applying correct migrations.

* Updated or rewrote deprecated code (like fixing url() import errors) to make it compatible.

* Used Django admin to manually add missing CMS pages and test the UI flow.

* For UI enhancements, explored the template structure and safely extended base.html without breaking layout logic.

This approach helped balance legacy compatibility with modern improvements like responsive design and interactive inputs.

**Note: for screen shots please view Screenshots.docx
