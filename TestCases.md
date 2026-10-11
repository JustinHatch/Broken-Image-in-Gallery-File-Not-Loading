# Gallery test cases

## Historical post-fix results

The following existing results are retained from the original project record. They describe the post-fix gallery, not a new test run. Original screenshot/project dates are unchanged.

| Test Case ID | Test Scenario                    | Steps to Reproduce                                         | Expected Result                          | Status |
| ------------ | -------------------------------- | ---------------------------------------------------------- | ---------------------------------------- | ------ |
| BIIGFNL-1    | Navigate to gallery page         | Open the website and go to the image gallery               | Gallery page loads without issues        | ✅ Pass |
| BIIGFNL-2    | Scroll through the gallery       | Scroll through the full list of gallery images             | All images load properly                 | ✅ Pass |
| BIIGFNL-3    | Identify broken image issue      | Stop at the image that previously failed to load           | Image is visible and displayed correctly | ✅ Pass |
| BIIGFNL-4    | Confirm image URL in source code | Inspect the broken image element and check its `src` value | Correct URL path should be visible       | ✅ Pass |
| BIIGFNL-5    | Verify post-fix gallery behavior | Reload the gallery after the fix                           | All images remain stable and functional  | ✅ Pass |


## Current demonstration scope

`broken_version.html` intentionally references the absent local file `missing-photo-4.jpg` for Photo 4. `fixed_version.html` uses the existing valid placeholder URL. The earlier `?text=Photo+4.jpg` URL only changed the generated label and could load successfully; the demonstration has been corrected without changing historical results.

To verify the maintained examples, open each file, check Photo 4, and inspect its `src`. The broken example should fail to load Photo 4; the fixed example should load it. Both examples use placeholder images and depend on third-party resources for the remaining images and styling.

The original failed investigation and later passed retest can be read in [TestRail evidence](Screenshots/broken%20image%20gala%203.png). That historical record is separate from the all-pass post-fix table above.
