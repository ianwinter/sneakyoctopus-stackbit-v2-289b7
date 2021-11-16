---
title: Home
layout: PageLayout
sections:
  - type: HeroSection
    elementId: homepage-hero-1
    colors: colors-a
    title: Helping you untangle the tentacles of technology.
    text: >
      Do you want to talk about SaaS, databases, pipelines, ML or web
      infrastructure? Maybe you want a site hosted or a basic template design
      site. Whatever it is I'll try and help.
    actions:
      - label: Let's talk
        altText: Let's talk
        url: '#contact'
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        elementId: ''
        type: Link
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-12
          - pr-8
          - pl-8
        alignItems: center
        justifyContent: center
        flexDirection: row
        borderRadius: none
        borderWidth: 0
        borderStyle: none
        borderColor: border-neutral
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: left
        margin:
          - mt-0
          - mb-12
      subtitle:
        fontWeight: '400'
        fontStyle: normal
        textAlign: left
        margin:
          - mt-0
          - mb-6
      text:
        textAlign: left
        margin:
          - mt-0
          - mb-8
      actions:
        justifyContent: flex-start
  - elementId: quote
    colors: colors-a
    quote: >
      > Talent without discipline is like an octopus on roller skates. There's
      plenty of movement, but you never know if it's going to be forward,
      backwards, or sideways.
    name: 'H. Jackson Brown, Jr.'
    backgroundImage:
      url: ''
      altText: ''
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
          - pl-24
          - pr-24
        alignItems: center
        justifyContent: center
      quote:
        textAlign: left
      name:
        fontWeight: 400
        fontStyle: normal
        textAlign: left
      title:
        fontWeight: 400
        fontStyle: normal
        textAlign: left
    type: QuoteSection
  - type: FeaturedPostsSection
    variant: variant-b
    colors: colors-a
    title: Recent work
    posts:
      - content/pages/blog/post-three.md
      - content/pages/blog/post-two.md
      - content/pages/blog/post-one.md
      - content/pages/blog/post-four.md
      - content/pages/blog/post-five.md
      - content/pages/blog/post-six.md
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-12
          - pr-8
          - pl-8
        justifyContent: center
        borderRadius: none
        borderColor: border-primary
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: center
      subtitle:
        fontWeight: '400'
        fontStyle: normal
        textAlign: center
        margin:
          - mt-0
          - mb-12
      actions:
        justifyContent: center
    subtitle: Explore case studies
  - elementId: contact
    colors: colors-a
    title: Contact me
    text: >
      Let’s work together on something great. Complete the form or send me an
      email at <hello@sneakyoctopus.co>. I look forward to hearing from you.
    form:
      type: FormBlock
      elementId: contact-form
      action: /.netlify/functions/submission_created
      destination: ''
      fields:
        - type: TextFormControl
          name: name
          label: Name
          placeholder: Your name
          isRequired: true
          width: 1/2
        - type: EmailFormControl
          name: email
          label: Email
          placeholder: Your email
          isRequired: true
          width: 1/2
        - name: looking-for
          label: What services are you looking for?
          defaultValue: Please choose...
          options:
            - Hosting
            - Wordpress
            - Technology advice
            - Something else
          isRequired: false
          width: full
          type: SelectFormControl
        - name: message
          label: Message
          placeholder: Your message
          isRequired: true
          width: full
          type: TextareaFormControl
        - name: consent
          label: >-
            I understand that this form is storing my submitted information so I
            can be contacted.
          isRequired: true
          width: full
          type: CheckboxFormControl
      submitLabel: Send Message
    feature:
      type: ImageBlock
      url: /images/danielle-macinnes-IuLgi9PWETU-unsplash.jpg
      altText: Contact us
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        fontWeight: 700
        fontStyle: normal
        textAlign: left
      text:
        textAlign: left
        margin:
          - mt-4
    action: /.netlify/functions/submission_created
    type: ContactSection
---
