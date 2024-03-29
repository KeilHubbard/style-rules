# style-rules
Style Rules to be used on all projects...  
With noted exceptions based on the project language. (ie. Python styles may be different than C)


### Project Names

  `Capitalized With Spaces`

### Repository Names

  `lowercase-with-hyphens`
  
### Branch Names

#### Regular (Persistant) Branches
+ Code Branches
  ```
  'main'
      Stable, Tested Release. Available to All End Users
  'beta'
      Next Planned Release, Available to Beta Test Users Only as Extended UAT
  'dev'
      Shared Version Branch of Current Sprint, the code branch used by 'qa' and 'uat'
  ```
+ Review/ Test Branches  
Absolutely NO Code or Documentation Changes may be Made in the following Branches
  ```
  'qa'
      Review within development parameters and within code to ensure code Quality, 
      Readability, Efficiency and Functionality meets requirements.
  'uat'
      "User Acceptance Testing"
      Internal review of End User experience 
      Per Requirements Documentation and User Stories
      May Be Released to a small group of known "True End Users" as "Alpha"
  ```

+ Working/ Ephemeral Branches

    + Specify Goal Of Branch:

    + Identify Related Ticket/ User Story/ Source

### Commits  

#### Messages

+ Specify the type of commit:
  ```
  feat: A new feature you're adding to a particular application
  fix: A bug fix
  imp: An Improvement to an existing feature
  style: Feature and updates related to styling
  refactor: Refactoring a specific section of the codebase
  test: Everything related to testing
  doc: Everything related to documentation
  chore: Regular code maintenance.
  ```
  + Capitalize subject line
  + Do not end subject line with period
  + Imperative Mood
  ```
  Example commit messages:

  git commit -m "fix: Fix bug causing electrical fires"
  git commit -m "imp: Decrease time to re-open websocket gateway"
  ```

#### Descriptions

### Package Names

`lowercase_with_underscores`

### Class & Object Names

`CapitalizedCamelCase`

+ Nouns in Class and Object Names ONLY
    + ie. PulseWidthCalculator

### Method & Function Names

`lowerCamelCase`

+ Start with descriptive Verb
   + ie. readActivePulseWidth()

### Variable Names

  `CONSTANT_VALUE_NOUN`
  
  `mutableVariableNoun`

### Brackets, Whitespace, and Line Width
+ Vertically Alligned Braces for Java, C, and other C-like languages  
+ Multiples of Four(4) **SPACES** for indentation. Tabs not to be used unless absolutely neccesary (ie. makefiles)
+ Other Whitespace used as determined helpful for readability  
+ Line widths to be limited to One Hundred and Twenty(120) characters wherever possible
```
  if (currentPulseWidth == lastPulseWidth)
  {
      for(int sample = 0, sample < 5000, sample++)
      {
          ...
      }
  }
  else
  {
      lastPulseWidth = currentPulseWidth;
  }
```
### Comments

+ Docstrings  
All Classes, Objects, Structs, and Functions/ Methods **MUST** include at-least a minimal docstring addressing the following:  
  + Main Description  
  + Parameters (Name, Data-Type, If Required or Optional, Description, Default Value)  
  + Return (Data-Type, Description, Failure Value)  
      
+ Inline & Multi-line Comments  
  + Other comments should be included only when determined neccesary to document processes that are not clearly defined in code  
  + When writing these comments first determine if the code cannot be better at "self-documenting" (ie. improved variable, function, or class names)  

### Versioning
Use standard semantic versioning (https://semver.org/)
