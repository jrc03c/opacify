# Intro

This tool stretches opacity to its maximum value in images that support transparency. For example, if the max opacity level of a particular image is 20%, then this tool multiples all of the alpha values by 5 so that the max opacity becomes 100%, and all of the other opacity values are scaled proportionally.

![example w/ birbs](https://i.ibb.co/4stTR1M/birds.png)

Note, though, that the tool currently doesn't stretch alpha values to fit the full range from 0% to 100%; i.e., it scales them up to 100%, but it does _not_ scale them down to 0%. For example, if all alpha values in an image fell between 25% and 50%, then stretching the alpha values to fit the entire range of 0% to 100% would require subtracting 25% from all values and then multiplying them all by 4. However, the current version would _only_ multiply all alpha values by 2 since doing so would cause the max alpha value to be 100%. I may add the option to stretch alpha values to the full range in the next iteration.

# Usage

Visit [https://ameyama.com/opacify](https://ameyama.com/opacify).
