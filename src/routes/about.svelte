
<script lang="ts">
  import { Accordion, AccordionItem } from 'sveltestrap';
    import {
    Button,
    Card,
    CardBody,
    CardFooter,
    CardHeader,
    CardSubtitle,
    CardText,
    CardTitle
  } from 'sveltestrap';
</script>
<div class="container mx-auto">
<div class="grid grid-cols-2 gap-4">
  


<Accordion>
  <AccordionItem active header="Home"><i class="bi bi-pin"></i>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Et vel adipisci voluptatibus natus odit facere tempore, sed corrupti ipsa vero modi nihil, nulla, sint voluptatem itaque harum ea debitis minima.</AccordionItem>
 
  <AccordionItem header="School">
    <a href="#home">Buena Vista Elementary</a>
  </AccordionItem>
 
  <AccordionItem header="Library">UCSB Library</AccordionItem>

</Accordion>

<Card class="mb-3">
  <CardHeader>
    <CardTitle>Card title</CardTitle>
  </CardHeader>
  <CardBody>
    <CardSubtitle>Card subtitle</CardSubtitle>
    <CardText>
      Some quick example text to build on the card title and make up the bulk of
      the card's content.
    </CardText>
    <Button>Button</Button>
  </CardBody>
  <CardFooter>Footer</CardFooter>
</Card>
</div>
</div>

