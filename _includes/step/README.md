{{ include step/*step-name* }}
-------------------------------
Steps are intended to be reusable chunks of text, worded and formatted to be included in multiple instuction pages.



As a step grows it can become a page by creating a md that contains just that include and/or can be reduced in size by having chunks removed and replaced with an include to the removed text in a new smaller include if required.

includes generally start with a #### to give them a heading if a step is upgraded to a page it is best to start with a ## and when that step is used in a chain of steps the include code can be prefixed ## as these hashes will be prepended to the existing ## resulting in the original ####
