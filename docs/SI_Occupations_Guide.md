# Site Index: Guide to Occupation Types and Subtypes 

We will tag `<occupation>` elements as self-closed with `@type` and `@subtype` attributes. We will required the `@type` attribute and make `@subtype` optional, and keyed to specific types. There should be no whitespaces in any of these values.

An example entry: 

```
  <occupation type="artist" subtype="painter"/>
```

Example with multiple white-space-separated subtypes:

```
   <occupation type="literary" subtype="poet essayist critic"/>
```

## Types and their subtypes:

* `type="artist"`
`subtype="..."`

    * painter (designate type of painter as appropriate in the `<note>` element, not in this element. 
    * printmaker (this includes printmaking for books)
    * engraver (this includes engravings for books)
    * sculptor
    * architect (for buildings)
    * landscape (for designers and planners of gardens. The occupation of gardener, for one who helps maintain a garden, is an `@type="service"` (see below).
    * illustrator (this includes book illustrators)

* `type="bookProducer"`
`subtype="..."`

    * publisher
    * printer (Do not use for art printing. For that, use `type="artist"` and choose subtype of printmaker, engraver, etc.) -->
    * binder
    * bookseller
           
* `type="religious"` 
`subtype="..."`
(Vicar and curate are the correct term within the Church of England; dissenters may use minister; if you are not sure of the correct term, use clergy. More specific titles go under roleName. (ie, Bishop of Dromore.) Thus far, we've mostly just used clergy for these.)

    * clergy
    * prophet
    * vicar
    * curate
    * minister
    * priest (Use for Catholic clergy as well as Greek/Roman clergy. Do not use priestess.)

* `type="educator"` 
`subtype="..."` 

    * teacher
    * schoolHead (for headmistress, schoolmaster, etc)
    
* `type="scholar"` 
`subtype="..."` 
(The occupation type "scholar" can be used for adults and children whose primary task is to study. This is the term used in censuses.)

    * philosopher (as distinct from natural philosopher, included in naturalist)
    * naturalist (covers the natural sciences and earth sciences, and includes biologist, botanist, ornithologist, geologist, etc.)
    * astronomer
    * curator (for libraries, museums, antiquarian collectors)
    * antiquarian (for one who researches artifacts rather than collects them)
    * inventor
    * historian
    * economist
    * agronomist (for those who study agriculture)
    
* `type="explorer"` 
`subtype="..."`  (includes occupations associated with travel, commerce, empire expansion) 

    * traveller 
    * navigator
    * cartographer
    * seaCaptain (commands a ship; distinct from military post)

* `type="legal"` 
`subtype="..."` (Note: specific titles go in `<roleName>`, not occupation. Do not use "lawyer" unless the person is actually American.)

    * barrister (British lawyers who can plead in court)
    * solicitor (most other categories of British lawyer)
    * lawyer (ONLY appropriate if from the United States) 
    * recorder
    * judge (ex: Mr. Justice Talfourd)
    * magistrate (ex: George Mitford)
           
* `type="literary"` 
`subtype="..."` 

    * novelist
    * poet
    * playwright
    * essayist (use for essayists who are not primarily writing specific literary/art reviews, but more broad-ranging philosophical or aesthetic writings)
    * critic (use for literary, theatre / art critics and reviewers)
    * journalist
    * editor
    * biographer
    * autobiographer
    * lexicographer
    * linguist (for someone who systemically studies languages, not simply a translator
    * translator

* `type="theater"` 
`subtype="..."`  

    * actor (general term for all sexes; do not use "actress".)
    * singer (for opera singers in performing roles)
    * manager (for actor-managers and theater managers like William Macready)
    * owner 
    * designer (for production designers, costume-makers, makers of stage sets and props)
    * musician (for pit players of music supporting the stage)
    * composer (for writers of instrumental and vocal music for the stage, including lyricists and librettists)

                     
* `type="medical"` 
`subtype="..."`  
(These terms are used in conjunction throughout the 19th c., so use more than one if necessary or if it's unclear, just use the main type "medical". For example,  use "apothecary" and "surgeon" for someone listed in a directory as an apothecary-surgeon. Don't use "doctor" here; put such titles under roleName.)
    * physician
    * surgeon (includes barbers and others who do surgery and bloodletting)
    * apothecary (use for pharmacy specialists)
    * midwife (includes, should we ever see one, a "man-midwife" or a male who assists with births and is not a physician or surgeon)
    * oculist
               
* `type="military"` 
`subtype="..."`  (Note: specific military titles belong in `<roleName>`.)

    * army
    * navy
                     
* `type="benevolence"` 
`subtype="..."` 

    * philanthropist (use for benevolent activites outside of the arts)
    * patron (use for supporters of the arts, theatre, and writers) 
                 
                  
                  <!-- POLITICAL & GOVERNMENT OCCUPATIONS: Use use "government" plus any of these:-->
                  <occupation>politician</occupation><!-- Use for elected officials and those running for election or who are in office by reason of political party or affiliation. Put their TITLE under <roleName></roleName>; ie, Member of Parliament for Westminster. -->
                  <occupation>orator</occupation><!-- Mostly use for political or reformist orators who are NOT clergy or actors -->
                  <occupation>reformer</occupation><!-- any public advocate for political or social reform -->
                  
                  
                     <occupation>monarch</occupation><!-- do not use king, queen, princess; put those titles under <roleName> instead -->
                     <occupation>courtier</occupation><!-- use for aristocracy and others whose job is to serve at court in some capacity. -->
                     <occupation>diplomat</occupation>
                     <occupation>ambassador</occupation><!-- In some cases, this occupation is also a roleName. ie, Ambassador to the Court of St. James.-->
                     <occupation>administrator</occupation><!-- Use for management positions, upper civil service positions within the British empire, etc. Lower positions may go under "clerk." "Civil servant" and bureaucrat are dispreferred.-->
                     
    
                     * clerk
                     <occupation>tax collector</occupation>
                     <occupation>postmaster</occupation>
                  
                  <!-- SERVICE OCCUPATIONS: Use "service" plus any of these: THus far, we've mostly used servant for all of these.-->
                     <occupation>service</occupation>
                        <occupation>servant</occupation>
                        <occupation>butler</occupation>
                        <occupation>maid</occupation>
                        <occupation>footman</occupation>
                        <occupation>cook</occupation>
                        <occupation>housekeeper</occupation>
                  
            
                  
                  <!-- TRADES, MERCHANTS, and AGRICULTURE-->
                     <occupation>trades</occupation>
                        <occupation>baker</occupation>
                        <occupation>bricklayer</occupation>
                        <occupation>wheelwright</occupation>
                        <occupation>carpenter</occupation>
                        <occupation>watchmaker</occupation>
                        <occupation>miller</occupation>
                        <occupation>goldsmith</occupation>
                        <occupation>jeweller</occupation>
                        <occupation>saddler</occupation>
                        <occupation>bootmaker</occupation>
                        
                    <occupation>blacksmith</occupation>

<occupation>innkeeper</occupation>
                  
                  <occupation>merchant</occupation><!-- prefer merchant to shopkeeper -->
                  <occupation>clerk</occupation>
                  <occupation>banker</occupation><!-- prefer to banking -->
                  <occupation>stockbroker</occupation>
                  <occupation>auctioneer</occupation>
                  <occupation>gambler</occupation>
                  
                  <occupation>farmer</occupation>