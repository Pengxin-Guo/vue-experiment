<template>
  <div>
    <form>
      <input type="text" v-model="user.name" />
      <br />
      <label> <input type="radio" v-model="user.sex" value="male" />男 </label>
      <label>
        <input type="radio" v-model="user.sex" value="female" />女
      </label>
      <br />
      <template v-for="(c, index) in courses">
        <label :key="`l${index}`">
          <input
            type="checkbox"
            v-model="user.courses"
            :value="{ id: c.id }"
            :key="index"
          />
          {{ c.name }}
        </label>
        <br :key="`b${index}`" />
      </template>
      <br />
      <br />
      <select v-model="user.title">
        <option v-for="(t, index) in titles" :key="index" :value="t.id">
          {{ t.name }}
        </option>
      </select>
      <br />
      <button type="button">提交</button>
    </form>
    <p>{{ user }}</p>
  </div>
</template>

<script>
export default {
  data: () => ({
    user: {
      name: null,
      sex: null,
      courses: [],
      title: null
    },

    titles: [
      { id: 1, name: "讲师" },
      { id: 2, name: "副教授" },
      { id: 3, name: "教授" }
    ],

    courses: [
      { id: 4, name: "Java", insertTime: "2019-03-05T20:20" },
      { id: 5, name: "Web开发技术", insertTime: "2019-04-17T08:00" },
      { id: 6, name: "系统程序设计", insertTime: "2019-05-05T12:40" }
    ]
  })
};
</script>
