<App>
  <View main>
    <Page>
      <Navbar title="List View"></Navbar>
      <BlockTitle>Simple List</BlockTitle>
      <List simpleList>
        <ListItem title="Item 1"></ListItem>
        <ListItem title="Item 2"></ListItem>
        <ListItem title="Item 3"></ListItem>
      </List>
      <BlockTitle>Simple Links List</BlockTitle>
      <List>
        <ListItem title="Link 1" link="#"></ListItem>
        <ListItem title="Link 2" link="#"></ListItem>
        <ListItem title="Link 3" link="#"></ListItem>
      </List>
      <BlockTitle>Data list, with icons</BlockTitle>
      <List>
        <ListItem title="Ivan Petrov" after="CEO">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem title="John Doe" badge="5">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem title="Jenna Smith">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
      </List>
      <BlockTitle>Links</BlockTitle>
      <List>
        <ListItem link="#" title="Ivan Petrov" after="CEO">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" title="John Doe" after="Cleaner">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" title="Jenna Smith">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
      </List>
      <BlockTitle>Links, Header, Footer</BlockTitle>
      <List>
        <ListItem link="#" header="Name" title="John Doe" after="Edit">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" header="Phone" title="+7 90 111-22-3344" after="Edit">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" header="Email" title="john@doe" footer="Home" after="Edit">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" header="Email" title="john@framework7" footer="Work" after="Edit">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
      </List>
      <BlockTitle>Links, no icons</BlockTitle>
      <List>
        <ListItem link="#" title="Ivan Petrov"></ListItem>
        <ListItem link="#" title="John Doe"></ListItem>
        <ListItem divider title="Divider Here"></ListItem>
        <ListItem link="#" title="Ivan Petrov"></ListItem>
        <ListItem link="#" title="Jenna Smith"></ListItem>
      </List>
      <BlockTitle>Grouped with sticky titles</BlockTitle>
      <List ul={false}>
        <ListGroup>
          <ListItem title="A" groupTitle></ListItem>
          <ListItem title="Aaron "></ListItem>
          <ListItem title="Abbie"></ListItem>
          <ListItem title="Adam"></ListItem>
        </ListGroup>
        <ListGroup>
          <ListItem title="B" groupTitle></ListItem>
          <ListItem title="Bailey"></ListItem>
          <ListItem title="Barclay"></ListItem>
          <ListItem title="Bartolo"></ListItem>
        </ListGroup>
        <ListGroup>
          <ListItem title="C" groupTitle></ListItem>
          <ListItem title="Caiden"></ListItem>
          <ListItem title="Calvin"></ListItem>
          <ListItem title="Candy"></ListItem>
        </ListGroup>
      </List>
      <BlockTitle>Mixed and nested</BlockTitle>
      <List>
        <ListItem link="#" title="Ivan Petrov" after="CEO">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" title="Two icons here">
          <svelte:fragment slot="media">
            <i class="icon demo-list-icon" />
            <i class="icon demo-list-icon" />
          </svelte:fragment>
        </ListItem>
        <ListItem title="No icons here"></ListItem>
        <li>
          <ul>
            <ListItem link="#" title="Ivan Petrov" after="CEO">
              <i slot="media" class="icon demo-list-icon" />
            </ListItem>
            <ListItem link="#" title="Two icons here">
              <svelte:fragment slot="media">
                <i class="icon demo-list-icon" />
                <i class="icon demo-list-icon" />
              </svelte:fragment>
            </ListItem>
            <ListItem title="No icons here"></ListItem>
            <ListItem link="#" title="Ultra long text goes here, no, it is really really long">
              <i slot="media" class="icon demo-list-icon" />
            </ListItem>
            <ListItem title="With toggle">
              <i slot="media" class="icon demo-list-icon" />
              <span slot="after">
                <Toggle />
              </span>
            </ListItem>
          </ul>
        </li>
        <ListItem link="#" title="Ultra long text goes here, no, it is really really long">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem title="With toggle">
          <i slot="media" class="icon demo-list-icon" />
          <span slot="after">
            <Toggle />
          </span>
        </ListItem>
      </List>
      <BlockTitle>Mixed, inset</BlockTitle>
      <List>
        <ListItem link="#" title="Ivan Petrov" after="CEO">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" title="Two icons here">
          <svelte:fragment slot="media">
          <i class="icon demo-list-icon" />
          <i class="icon demo-list-icon" />
          </svelte:fragment>
        </ListItem>
        <ListItem link="#" title="Ultra long text goes here, no, it is really really long">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem title="With toggle">
          <i slot="media" class="icon demo-list-icon" />
          <span slot="after">
            <Toggle />
          </span>
        </ListItem>
        <div class="block-footer" slot="after-list">
          <p>Here comes some useful information about list above</p>
        </div>
      </List>
      <BlockTitle>Tablet inset</BlockTitle>
      <List mediumInset>
        <ListItem link="#" title="Ivan Petrov" after="CEO">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <ListItem link="#" title="Two icons here">
          <svelte:fragment slot="media">
          <i class="icon demo-list-icon" />
          <i class="icon demo-list-icon" />
          </svelte:fragment>
        </ListItem>
        <ListItem link="#" title="Ultra long text goes here, no, it is really really long">
          <i slot="media" class="icon demo-list-icon" />
        </ListItem>
        <div class="block-footer" slot="after-list">
          <p>This list block will look like "inset" only on tablets (iPad)</p>
        </div>
      </List>

      <BlockTitle>Media Lists</BlockTitle>
      <Block>
        <p>Media Lists are almost the same as Data Lists, but with a more flexible layout for visualization of more complex data, like products, services, users, etc.</p>
      </Block>
      <BlockTitle>Songs</BlockTitle>
      <List mediaList>
        <ListItem
          link="#"
          title="Yellow Submarine"
          after="$15"
          subtitle="Beatles"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus."
        >
          <img slot="media" src="https://cdn.framework7.io/placeholder/people-160x160-1.jpg" width="80" />
        </ListItem>
        <ListItem
          link="#"
          title="Don't Stop Me Now"
          after="$22"
          subtitle="Queen"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus."
        >
          <img slot="media" src="https://cdn.framework7.io/placeholder/people-160x160-2.jpg" width="80" />
        </ListItem>
        <ListItem
          link="#"
          title="Billie Jean"
          after="$16"
          subtitle="Michael Jackson"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus."
        >
          <img slot="media" src="https://cdn.framework7.io/placeholder/people-160x160-3.jpg" width="80" />
        </ListItem>
      </List>
      <BlockTitle>Mail App</BlockTitle>
      <List mediaList>
        <ListItem
          link="#"
          title="Facebook"
          after="17:14"
          subtitle="New messages from John Doe"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus."
        ></ListItem>
        <ListItem
          link="#"
          title="John Doe (via Twitter)"
          after="17:11"
          subtitle="John Doe (@_johndoe) mentioned you on Twitter!"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus."
        ></ListItem>
        <ListItem
          link="#"
          title="Facebook"
          after="16:48"
          subtitle="New messages from John Doe"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus."
        ></ListItem>
        <ListItem
          link="#"
          title="John Doe (via Twitter)"
          after="15:32"
          subtitle="John Doe (@_johndoe) mentioned you on Twitter!"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sagittis tellus ut turpis condimentum, ut dignissim lacus tincidunt. Cras dolor metus, ultrices condimentum sodales sit amet, pharetra sodales eros. Phasellus vel felis tellus. Mauris rutrum ligula nec dapibus feugiat. In vel dui laoreet, commodo augue id, pulvinar lacus."
        ></ListItem>
      </List>
      <BlockTitle>Something more simple</BlockTitle>
      <List mediaList>
        <ListItem
          title="Yellow Submarine"
          subtitle="Beatles">
          <img slot="media" src="https://cdn.framework7.io/placeholder/fashion-88x88-1.jpg" width="44" />
        </ListItem>
        <ListItem
          link="#"
          title="Don't Stop Me Now"
          subtitle="Queen">
          <img slot="media" src="https://cdn.framework7.io/placeholder/fashion-88x88-2.jpg" width="44" />
        </ListItem>
        <ListItem
          title="Billie Jean"
          subtitle="Michael Jackson">
          <img slot="media" src="https://cdn.framework7.io/placeholder/fashion-88x88-3.jpg" width="44" />
        </ListItem>
      </List>
      <BlockTitle>Inset</BlockTitle>
      <List mediaList inset>
        <ListItem
          link="#"
          title="Yellow Submarine"
          subtitle="Beatles">
          <img slot="media" src="https://cdn.framework7.io/placeholder/fashion-88x88-4.jpg" width="44" />
        </ListItem>
        <ListItem
          link="#"
          title="Don't Stop Me Now"
          subtitle="Queen">
          <img slot="media" src="https://cdn.framework7.io/placeholder/fashion-88x88-5.jpg" width="44" />
        </ListItem>
        <ListItem
          link="#"
          title="Billie Jean"
          subtitle="Michael Jackson">
          <img slot="media" src="https://cdn.framework7.io/placeholder/fashion-88x88-6.jpg" width="44" />
        </ListItem>
      </List>
    </Page>
  </View>
</App>
<style>
  :global(.demo-list-icon, .icon-f7) {
    background: #ccc;
    display: block;
    position: relative;
  }
  :global(.ios .demo-list-icon, .ios .icon-f7, .ios .icon-vi) {
    width: 29px;
    height: 29px;
    border-radius: 6px;
    box-sizing: border-box;
  }
  :global(.md .demo-list-icon, .md .icon-f7, .md .icon-vi) {
    width: 24px;
    height: 24px;
    border-radius: 4px;
  }
  :global(.aurora .demo-list-icon, .aurora .icon-f7, .aurora .icon-vi) {
    width: 18px;
    height: 18px;
    border-radius: 4px;
  }
</style>
<script>
  import {App, View, Page, Navbar, BlockTitle, List, ListItem, Icon, ListGroup, Toggle, BlockFooter, Block} from 'framework7-svelte';
</script>
