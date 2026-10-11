# Broken Image in Gallery — QA Demonstration

An existing manual QA project demonstrating how to investigate an image-loading issue, inspect the image reference, document a defect, and verify a correction using Jira and TestRail.

## Broken and fixed examples

- [Broken gallery](broken_version.html): Photo 4 intentionally references the missing local file `missing-photo-4.jpg`.
- [Fixed gallery](fixed_version.html): Photo 4 uses the existing working placeholder URL.

Open each file in a browser to compare the behavior. These are demonstration galleries using placeholder images, not the original client's photographs. The earlier broken example used `?text=Photo+4.jpg`, which changes placeholder text rather than causing a load failure. That example has been corrected; historical screenshots and project dates remain unchanged.

## QA evidence

- [Original post-fix test-case results and scope notes](TestCases.md)
- [TestRail case](Screenshots/broken%20image%20gala%201.png)
- [TestRail expected result](Screenshots/broken%20image%20gala%202.png)
- [TestRail failed result and passed retest](Screenshots/broken%20image%20gala%203.png)
- [Jira backlog](Screenshots/Broken%20Image%20gallery%20Jira%20flow%201.png), [task flow](Screenshots/Broken%20Image%20gallery%20Jira%20flow%202.png), and [completion](Screenshots/Broken%20Image%20gallery%20Jira%20flow%203.png)
- [Original gallery screenshot](Screenshots/image%20not%20loading.png)

Historical fail/pass entries belong to different stages of the investigation. They are not claims that every version or every current run passes.

## Repository contents

```text
broken_version.html
fixed_version.html
Screenshots/       # Original evidence; capitalization matches the directory
TestCases.md       # Original post-fix results and demonstration notes
README.md
```

Tools used: browser inspection, HTML editing, Jira, TestRail, and GitHub. Skills demonstrated: visual/functional testing, troubleshooting, defect documentation, and retesting. This is portfolio project experience.
