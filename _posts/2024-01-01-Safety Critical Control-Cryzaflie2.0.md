---
layout: post
author: Chongbo Zhao
tags: [overview, moonwalk]
---

 Autonomous collision avoidance requires accurate environmental perception; however, flight systems often possess limited sensing capabilities with field-of-view (FOV) restrictions. To navigate this challenge, we present a safety-aware approach for online determination of the optimal sensor-pointing direction ψd which utilizes control barrier functions (CBFs). First, we generate a spatial density function Φ which leverages CBF constraints to map the collision risk of all local coordinates. Then, we convolve Φ with an attitude-dependent sensor FOV quality function to produce the objective function Γ which quantifies the total observed risk for a given pointing direction. Finally, by finding the global optimizer for Γ, we identify the value of ψd which maximizes the perception of risk within the FOV. We incorporate ψd into a safety-critical flight architecture and conduct a numerical analysis using multiple simulated mission profiles. Our algorithm achieves a success rate of 88−96%, constituting a 16−29% improvement compared to the best heuristic methods. We demonstrate the functionality of our approach via a flight demonstration using the Crazyflie 2.1 micro-quadrotor. Without a priori obstacle knowledge, the quadrotor follows a dynamic flight path while simultaneously calculating and tracking ψd to perceive and avoid two static obstacles with an average computation time of 371 μs.[^1]


# Sample heading 1
## Sample heading 2
### Sample heading 3
#### Sample heading 4
##### Sample heading 5
###### Sample heading 6

Mauris viverra dictum ultricies. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod.

## Lists

Unordered:

- Fusce non velit cursus ligula mattis convallis vel at metus[^2].
- Sed pharetra tellus massa, non elementum eros vulputate non.
- Suspendisse potenti.

Ordered:

1. Quisque arcu felis, laoreet vel accumsan sit amet, fermentum at nunc.
2. Sed massa quam, auctor in eros quis, porttitor tincidunt orci.
3. Nulla convallis id sapien ornare viverra.
4. Nam a est eget ligula pellentesque posuere.

## Blockquote

The following is a blockquote:

> Suspendisse tempus dolor nec risus sodales posuere. Proin dui dui, mollis a consectetur molestie, lobortis vitae tellus.

## Thematic breaks (<hr>)

Mauris viverra dictum ultricies[^3]. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. **You can put some text inside the horizontal rule like so.**

---
{: data-content="hr with text"}

Mauris viverra dictum ultricies. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. **Or you can just have an clean horizontal rule.**

---

Mauris viverra dictum ultricies. Vestibulum quis ipsum euismod, facilisis metus sed, varius ipsum. Donec scelerisque lacus libero, eu dignissim sem venenatis at. Etiam id nisl ut lorem gravida euismod. Or you can just have an clean horizontal rule.

## Code

Now some code:

```
const ultimateTruth = 'follow middlepath';
console.log(ultimateTruth);
```

And here is some `inline code`!

## Tables

Now a table:

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

## Images

![theme logo](http://www.abhinavsaxena.com/images/abhinav.jpeg)

This is an image[^4]

---
{: data-content="footnotes"}

[^1]: Bena, Ryan M., Chongbo Zhao, and Quan Nguyen. "[Safety-Aware Perception for Autonomous Collision Avoidance in Dynamic Environments][Safety-Aware]." IEEE Robotics and Automation Letters (2023). 
[Safety-Aware]: https://doi.org/10.48550/arXiv.2403.13929
[^2]: hey there, don't forget to read all the footnotes!
[^3]: this is another footnote.
[^4]: this is a very very long footnote to test if a very very long footnote brings some problems or not; hope that there are no problems but you know sometimes problems arise from nowhere.
