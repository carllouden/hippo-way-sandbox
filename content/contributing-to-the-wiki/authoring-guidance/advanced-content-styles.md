---
id: d3377b2c-2eb7-4da3-a5b6-bfcc9c92b757
title: Advanced content styles
order: 2
tags:
  - Styleguide
  - Authoring
  - Guidance
  - Contributing
  - newtag
back:
  - /contributing-to-the-wiki#creating-content-for-the-wiki
  - creating content for the Wiki
isDirectory: false
---

<Standout>
  <p>An overview of the custom styles and components supported by the Hippo Wiki to add richer content presentation than standard Markdown.</p>
</Standout>

The [core content styles](content-styles) provided by Markdown are relatively basic but can be extended using custom components. Once a need is identified, custom components are designed, developed and integrated into the Wiki codebase, and can then be used in Markdown in a similar way to using standard HTML elements.

Custom components often have optional parameters that can be used to affect the rendered outcome on a page. Using these components is more complex than writing standard Markdown but using the documentation and examples provided should enable most content authors to benefit from the extra functionality.

## Accordion

### Outcome and usage example

<Accordion>
  <AccordionSection title={"Further reading about this topic"}>
    <p>
      Example content, written in Markdown as usual.

      * Lists
      * Like this 

    </p>
  </AccordionSection>
  <AccordionSection title={"Stuff you shouldn't bother reading about this topic"}>
    <p>
      Example content, written in Markdown as usual.

      * Lists
      * Like this 

    </p>
  </AccordionSection>
</Accordion>

<Details summary={"Usage example"}>
  ```
  <Accordion>
    <AccordionSection title={"Further reading about this topic"}>
      <p>
        Example content, written in Markdown as usual.

        * Lists
        * Like this 

      </p>
    </AccordionSection>
    <AccordionSection title={"Stuff you shouldn't bother reading about this topic"}>
      <p>
        Example content, written in Markdown as usual.

        * Lists
        * Like this 

      </p>
    </AccordionSection>
  </Accordion>
  ```
</Details>

### Instructions for use

1. Add an opening tag: `<Accordion>`
1. Add an opening and closing tag for an expandable accordion section:  
`<AccordionSection></AccordionSection>`
1. Add a clickable title to the section's opening tag using the **title** property:  
`<AccordionSection title="Meaningful title here">`
1. Add the content that will be shown when the item is expanded by adding markdown between the tags:  
`<AccordionSection title="Meaningful title here">Markdown content here</AccordionSection>`
1. Add as many expandable sections as required by repeating steps 2 - 4
1. Add a closing tag to complete the component: `</Accordion>`

## Card

### Outcome and usage example

#### Standard card

##### Size: Extra large (XL)

<CardContainer size="XL">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer size="XL">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>
```
</Details>

##### Size: Large (L)

<CardContainer size="L">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer size="L">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>
```
</Details>

##### Size: Medium (M)

<CardContainer size="M">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer size="M">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>
```
</Details>

##### Size: Small (S)

<CardContainer size="S">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer size="S">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>
```
</Details>

##### Size: Two columns (2)

<CardContainer size="2">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer size="2">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>
```
</Details>

##### Size: Three columns (3)

<CardContainer size="3">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer size="3">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>
```
</Details>

##### Size: Four columns (4)

<CardContainer size="4">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer size="4">
  <Card title="Hippo website" link="https://www.hippodigital.co.uk">This is a link to the Hippo website in the default colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="blue">This is a link to the Hippo website in the blue colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="turquoise">This is a link to the Hippo website in the turquoise colour</Card>
  <Card title="Hippo website" link="https://www.hippodigital.co.uk" color="pink">This is a link to the Hippo website in the pink colour</Card>
  <Card title="Hippo website">This card is not linked and is in the default colour</Card>
  <Card title="Hippo website" color="blue">This card is not linked and is in the blue colour</Card>
  <Card title="Hippo website" color="turquoise">This card is not linked and is in the turquoise colour</Card>
  <Card title="Hippo website" color="pink">This card is not linked and is in the pink colour</Card>
</CardContainer>
```
</Details>

#### Chevron cards

<CardContainer style="chevrons" size="M">
  <Card title="Communities and support" link="#">Access guidance for key aspects of the GDS delivery model, including service assessments</Card>
  <Card title="Community workstreams" link="#">Explore emrging technologies like AI and key topics that are shaping the research profession</Card>
  <Card title="Research tools and services" link="#">Find out how and when to craft impactful case studies</Card>
  <Card title="Development and progression" link="#">Something else about this other essential research topic</Card>
</CardContainer>

<Details summary={"Usage example"}>
```
<CardContainer style="chevrons">
  <Card title="Communities and support" link="#">Access guidance for key aspects of the GDS delivery model, including service assessments</Card>
  <Card title="Community workstreams" link="#">Explore emrging technologies like AI and key topics that are shaping the research profession</Card>
  <Card title="Research tools and services" link="#">Find out how and when to craft impactful case studies</Card>
  <Card title="Development and progression" link="#">Something else about this other essential research topic</Card>
</CardContainer>
```
</Details>

### Instructions for use

1. Add an opening tag: `<CardContainer>`
2. Optionally, set the size of the list with the **size** property:  
`<CardContainer size="M">`  
*Supports: S, M, L (default), XL, 2, 3, 4*
1. Add an opening and closing tag for each card: `<Card></Card>`
1. Add a title to the card's opening tag using the **title** property:  
`<Card title="Meaningful title here"></Card>`
1. Add content to the card by including the content between the tags:  
`<Card title="Meaningful title here">Markdown content here</Card>`
1. For clickable cards, use the **link** property to specify where the link goes to:  
`<Card title="Meaningful title here" link="https://www.hippodigital.com/">Markdown content here</Card>` 
1. Optionally, set the card's hover colour using the **color** property:  
`<Card title="your title here" link="https://www.google.com/" color="blue">Your content here</Card>`  
*Supports: default (default), blue, turquoise and pink*
1. Add as many cards as required following steps 2 - 6
2. Add a closing tag to complete the component: `</CardContainer>`

## Custom link

### Outcome and usage example

#### With custom text

<CustomLink url="/working-at-hippo" text="This is the link text" />

<Details summary={"Usage example"}>
```
<CustomLink url="/working-at-hippo" text="This is the link text" />
```
</Details>

#### With type but no custom text

<CustomLink url="/working-at-hippo" type="more" />

<Details summary={"Usage example"}>
```
<CustomLink url="/working-at-hippo" type="more" />
```
</Details>

### Instructions for use

1. Add a self-closing opening tag: `<CustomLink />`
2. Add a url to the opening tag using the **url** property:  
`<CustomLink url="/working-at-hippo">`
1. Usually you'll want to specify the link text using the **text** property: 
`<CustomLink url="/working-at-hippo" text="This is the link text" />`  
*Defaults to automated text if not provided*
1. Optionally, specify the type of link using the **type** property: 
`<CustomLink url="/working-at-hippo" type="more" />`  
*Supports: none (default), more*

## Details

### Outcome and usage example

<Details summary={"Further reading about this topic"}>
  Typically the content shown inside a Details component is more simplistic than that in an accordion component.

  However, the Details component also supports:

  * Lists
  * Other things
</Details>

<Details summary={"Usage example"}>
```
<Details summary={"This is the clickable text that opens the component"}>
  Add any valid Markdown content here, including text, lists, images, etc.
</Details>
```
</Details>

### Instructions for use

1. Add an opening tag: `<Details>`
2. Add a clickable title to the opening tag using the **summary** property: `<Details summary="Meaningful title here">`
3. Add the content that will be shown when the Details item is expanded by adding markdown after the `<Details>` tag: `<Details summary="Meaningful title here">Markdown content here</Details>`
4. Add a closing tag to complete the component: `</Details>`

## Page list

To minimise manual editing and errors, all pages in a directory can be listed automatically. This is especially useful for directories of related pages, such as client pages, how to pages or Kimble guides.

### Outcome and usage example

#### Current clients (with multiple excluded directories)

<PageList dir="/working-on-projects/our-clients" exclude="previous-clients,project-insights" moreUrl="/working-on-projects/our-clients" moreText="All our clients" />

<Details summary={"Usage example"}>
```
  <PageList dir="/working-on-projects/our-clients" exclude="previous-clients,project-insights" moreUrl="/working-on-projects/our-clients" moreText="All our clients" />
```
</Details>

#### All clients (with A-Z separators and excluded directory)

<PageList dir="/working-on-projects/our-clients" sort="az" showAlphabetHeadings={true} exclude="project-insights" moreUrl="/working-on-projects/our-clients" moreText="All our clients" />

<Details summary={"Usage example"}>
```
  <PageList dir="/working-on-projects/our-clients" sort="az" showAlphabetHeadings={true} exclude="project-insights" moreUrl="/working-on-projects/our-clients" moreText="All our clients" />
```
</Details>

#### Marketing (with frontmatter sorting)

<PageList dir="/about-hippo/business-functions/marketing/" sort="order" />

<Details summary={"Usage example"}>
```
   <PageList dir="/about-hippo/business-functions/marketing/" sort="order" />
```
</Details>

#### Wiki help (with 'get started' tag)

<PageList dir="/contributing-to-the-wiki/frequent-tasks" tags="get started" />

<Details summary={"Usage example"}>
```
   <PageList dir="/contributing-to-the-wiki/frequent-tasks" tags="get started" />
```
</Details>

#### Current clients (limited to 12 shuffled, medium cards)

<PageList dir="/working-on-projects/our-clients" limit={12} exclude="previous-clients" sort="shuffle" display="cards" cardSize="M" moreUrl="/working-on-projects/our-clients" moreText="All our clients" />

<Details summary={"Usage example"}>
```
   <PageList dir="/working-on-projects/our-clients" limit={12} exclude="previous-clients" sort="shuffle" display="cards" cardSize="M" moreUrl="/working-on-projects/our-clients" moreText="All our clients" />
```
</Details>

### Instructions for use

1. Add the self-closing component to a page: `<PageList />`
1. Specify the full path to the directory of pages to be displayed with the **dir** property:  
`<PageList dir="/working-on-projects/our-clients" />`  
*If omitted, defaults to current page + '/archive' e.g. this-page/archive*
1. Optional: Limit the number of displayed results by specifying the **limit** property:
`<PageList dir="/working-on-projects/our-clients" limit={10} />`
1. Optional: Set the name of a subdirectory to exclude from the displayed list with the **exclude** property:  
`<PageList dir="/working-on-projects/our-clients" exclude="some-directory" />`
*Note: Separate multiple directories with commas `this-directory,that-directory`
*Note: Any individual pages with `order: exclude` in their frontmatter will also be excluded*
1. Optional: Set the sort order with the **sort** property:  
`<PageList dir="/working-on-projects/our-clients" sort="za" />`  
*Supports: az (default), za, shuffle, order*  
*Note: 'order' uses the 'order' defined in each page's frontmatter, and then falls back to a-z*
1. Optional: Set a tag to filter by with the **tag** property:  
`<PageList dir="/working-on-projects/our-clients" tags="featured" />`  
*Note: Filters to pages with the tag in its frontmatter e.g. tags: - featured*
*Note: Separate multiple tags with commas `this-tag,that-tag`
1. Optional: Set the display type using the **display** property:  
`<PageList dir="/working-on-projects/our-clients" display="cards" />`  
*Supports: ul (default), ol or cards*
1. Optional: Set the size of the list with the **size** property (currently only works with cards display type):  
`<PageList dir="/working-on-projects/our-clients" cardSize="M" />`  
*Supports: S, M, L (default)*
1. Optional: Set a link to another page, typically to show 'all pages', with the **more** property:  
`<PageList dir="/working-on-projects/our-clients" moreUrl="/working-on-projects/our-clients" />`  
1. Optional: Set the text of the more link with the **moreText** property:  
`<PageList dir="/working-on-projects/our-clients" moreUrl="/working-on-projects/our-clients" moreText="All our clients" />`  
*Default: More pages*

## Stack

The Stack component is used to present part of the page as related sections – by default, as columns. However, it can also be used to present sections as rows.

This might typically be used to show two or three columns of lists rather than having all the lists in sequential order in a page.

### Outcome and usage example

#### Row direction
<Stack separator>
  <section>
    ### Content guidance
    * [Writing for readability](/contributing-to-the-wiki/content-guidance/writing-guide)
    * [Structuring and formatting content](/contributing-to-the-wiki/content-guidance/formatting-guide)
    * [Using grammar and punctuation](/contributing-to-the-wiki/content-guidance/grammar-guide)
    * [Specific phrases and terminology](/contributing-to-the-wiki/content-guidance/terminology-guide)
  </section>
  <section>
    ### Styling and layout
    * [Main content styles](/contributing-to-the-wiki/authoring-guidance/content-styles)
    * [Advanced content styles](/contributing-to-the-wiki/authoring-guidance/advanced-content-styles)
  </section>
</Stack>

#### Column direction
<Stack direction="column" separator>
  <section>
    ### Content guidance
    * [Writing for readability](/contributing-to-the-wiki/content-guidance/writing-guide)
    * [Structuring and formatting content](/contributing-to-the-wiki/content-guidance/formatting-guide)
    * [Using grammar and punctuation](/contributing-to-the-wiki/content-guidance/grammar-guide)
    * [Specific phrases and terminology](/contributing-to-the-wiki/content-guidance/terminology-guide)
  </section>
  <section>
    ### Styling and layout
    * [Main content styles](/contributing-to-the-wiki/authoring-guidance/content-styles)
    * [Advanced content styles](/contributing-to-the-wiki/authoring-guidance/advanced-content-styles)
  </section>
</Stack>

#### Reversed row direction
<Stack direction="row-reverse" separator >
  <section>
    ### Content guidance
    * [Writing for readability](/contributing-to-the-wiki/content-guidance/writing-guide)
    * [Structuring and formatting content](/contributing-to-the-wiki/content-guidance/formatting-guide)
    * [Using grammar and punctuation](/contributing-to-the-wiki/content-guidance/grammar-guide)
    * [Specific phrases and terminology](/contributing-to-the-wiki/content-guidance/terminology-guide)
  </section>
  <section>
    ### Styling and layout
    * [Main content styles](/contributing-to-the-wiki/authoring-guidance/content-styles)
    * [Advanced content styles](/contributing-to-the-wiki/authoring-guidance/advanced-content-styles)
  </section>
</Stack>

#### Reversed column direction
<Stack direction="column-reverse" separator>
  <section>
    ### Content guidance
    * [Writing for readability](/contributing-to-the-wiki/content-guidance/writing-guide)
    * [Structuring and formatting content](/contributing-to-the-wiki/content-guidance/formatting-guide)
    * [Using grammar and punctuation](/contributing-to-the-wiki/content-guidance/grammar-guide)
    * [Specific phrases and terminology](/contributing-to-the-wiki/content-guidance/terminology-guide)
  </section>
  <section>
    ### Styling and layout
    * [Main content styles](/contributing-to-the-wiki/authoring-guidance/content-styles)
    * [Advanced content styles](/contributing-to-the-wiki/authoring-guidance/advanced-content-styles)
  </section>
</Stack>

<Details summary={"Usage example"}>
```
<Stack separator>
  <section>
    ### Markdown content
    * List item one
    * List item two
    * List item three
  </section>
  <section>
    ### Markdown content
    * List item one
    * List item two
  </section>
</Stack>
```
</Details>

### Instructions for use

1. Add an opening tag: `<Stack>`
2. Optionally, add a separator between sections using the **separator** property:  
`<Stack separator></Stack>`
1. Add an opening and closing HTML tag for each section:  
`<Stack separator><section></section></Stack>`
1. Add content to the card by including the content between the tags:  
`<Stack separator><section>Add content here as Markdown</section></Stack>`
1. Optionally, specify the layout of the stack using the **direction** property:  
`<Stack direction="column" separator></Stack>`  
Supports: row (default), row-reverse, column, column-reverse
1. Add as many sections as required following steps 3 - 5
2. Add a closing tag to complete the component: `</Stack>`

## Status

### Outcome and usage example

<Status status="discovery"/>
<Status status="alpha"/>
<Status status="beta"/>
<Status status="live"/>

<Details summary={"Usage example"}>
```
<Status status="discovery"/>
```
</Details>

### Instructions for use

1. Add the self-closing component to a page: `<Status/>`
2. Specify the status using the **status** property: `<Status status="live"/>`  
*Supports: discovery, alpha, beta and live*

## Summary list

### Outcome and usage example

<SummaryList>
  <SummaryListItem label="Name" value="Frank" />
  <SummaryListItem label="Age" value="50" />
  <SummaryListItem label="Location" value="London" />
</SummaryList>

<Details summary={"Usage example"}>
```
<SummaryList>
  <SummaryListItem label="Name" value="Frank" />
  <SummaryListItem label="Age" value="50" />
  <SummaryListItem label="Location" value="London" />
</SummaryList>
```
</Details>

### Instructions for use

1. Add an opening tag: `<SummaryList>`
1. Add a self-closing component for each row item: `<SummaryListItem />`
1. For each row item, add content using the **label** and **value** properties respectively:  
`<SummaryListItem label="Name" value="Jane Smith" />`
1. Add a closing tag to complete the component: `</SummaryList>`

## Table from data

For large or complex tables, structured data can be saved in a file and then passed to a table component in JSON or CSV format:

* JSON is a hugely popular data format that is returned by most APIs and can be extracted easily from a spreadsheet using a tool such as [opensheet](https://github.com/benborgers/opensheet#readme).
* CSV is a long-standing tabular data format that can be saved directly from a Google Sheet or Excel file.

### Outcome and usage example

<TableFromData file="/data/table-data-test.csv" dense />

<Details summary={"Usage example"}>
```
  <TableFromData file="/data/table-data-test.json" dense />
```
</Details>

### Instructions for use

1. Create a JSON or CSV data file with the extension `.json` or `.csv` respectively.
1. Validate the file contains a valid data structure using a [JSON validator](https://jsonlint.com/) or [CSV validator](https://csvlint.io/).
1. Save the file to the `/public/data/` folder.
1. Add the self-closing component to a page: `<TableFromData />`
1. Specify the data file using the **file** property:  
`<TableFromData file="/data/my-file.json" />`  
Note: Do not include the `/public` part of the path e.g. `/data/my-file.json`
1. For large tables, optionally use the `dense` property to show a more compact table:  
`<TableFromData file="/data/my-file.json" dense />`
