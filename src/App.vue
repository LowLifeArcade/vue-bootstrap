<template>
  <NavBar />

  <div class="container mb-4">
    <div class="row h-75">
      <nav class="col-3 bg-secondary text-white shadow-sm">
        <div class="container p-4">
          <NavItem :text="Home" />
          <div>Menu</div>
          <div>Directions</div>
          <div>Settings</div>
        </div>
      </nav>
      <section class="col-8">
        <div class="container bg-white h-75 mt-2">
          {{ counter }}
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cupiditate
          sunt fuga eaque unde pariatur molestiae laudantium. Quibusdam, unde
          dicta ipsa molestias dolor nobis, facere inventore laudantium
          deleniti, saepe numquam consectetur?
        </div>
      </section>
      <article class="col-8 p-2">
        <TasksComponent :tasks="tasks" />
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum et
        repellat velit molestiae amet, autem omnis harum explicabo dolorem quis
        quo facere laboriosam delectus nisi ad aspernatur nihil, blanditiis
        quae. Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi
        optio illo consequatur, facere in laudantium suscipit saepe blanditiis
        odit asperiores ducimus! Facere, incidunt minus sit sapiente iure
        reiciendis reprehenderit consequatur. Lorem ipsum dolor sit amet,
        consectetur adipisicing elit. Iste tenetur eaque quaerat. Consequuntur
        natus cumque provident adipisci atque quaerat commodi. Lorem ipsum dolor
        sit amet consectetur adipisicing elit. Provident impedit velit iusto.
        Aspernatur mollitia natus illum ducimus non debitis consectetur vitae,
        assumenda modi sed deleniti ad ipsam nobis esse vel exercitationem
        dolores atque laudantium voluptatem aliquid libero! Ducimus, quam, quis
        consectetur distinctio voluptate eius explicabo, excepturi magnam harum
        dolorum vero qui laudantium nemo culpa eum voluptatem recusandae
        corporis iste ad quo voluptatum nisi voluptatibus enim cum! Reiciendis
        sunt similique repudiandae fugiat soluta impedit officiis consectetur
        quod deleniti sequi, minima ipsam minus blanditiis! Officiis corporis
        laudantium consequuntur, molestiae quibusdam iusto aut atque iure soluta
        itaque saepe, nesciunt rerum totam modi omnis? Iste beatae eum assumenda
        aperiam tempora fugiat, laudantium porro placeat odio rem voluptas? At
        quae maiores dolor nesciunt tempora, est ex accusamus? Aut vel
        repudiandae fugiat magni molestias debitis blanditiis eius totam porro,
        commodi ab maiores quisquam iure inventore consectetur a dolores
        deserunt at veritatis eligendi fuga sit recusandae quaerat. Nobis, autem
        voluptates. Nulla quae eaque minima eius ut quaerat saepe. Dolorem,
        repellat! Voluptate alias aliquam hic temporibus eum repudiandae dolore
        nihil totam excepturi dignissimos quod nulla nemo iure, expedita rerum
        reprehenderit adipisci, ipsum id iusto. Ducimus nesciunt beatae error,
        earum distinctio rerum, atque natus quod asperiores voluptate alias a.
      </article>
      <aside class="col-4 bg-info p-4 mt-4 shadow h-25">
        <h2>Dear Reader</h2>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptate
        dolores culpa possimus excepturi, nulla provident rerum quia soluta
        doloremque consectetur consequatur quod! Velit soluta dicta possimus rem
        quam, aut ut.
      </aside>
    </div>
  </div>
  

  <FooterComponent />
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import NavBar from './components/NavBar.vue';
import NavItem from './components/NavItem.vue';
import TasksComponent from './components/TasksComponent.vue';

export default {
  name: 'App',
  components: {
    FooterComponent,
    NavBar,
    NavItem,
    TasksComponent,
  },
  data() {
    return {
      Home: 'Home',
      tasks: [],
    };
  },
  created() {
    this.tasks = [
      { id: 1, text: 'Stuff', day: 'Monday', reminder: true },
      { id: 2, text: 'Stuff', day: 'Tuesday', reminder: true },
      { id: 3, text: 'Stuff', day: 'Monday', reminder: true },
    ];
  },
};
</script>

<style>
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50; */
  /* margin-top: 60px; */
}
</style>
