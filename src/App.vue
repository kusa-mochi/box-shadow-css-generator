<template>
  <div id="app">
    <table class="shadow-settings">
      <tbody>
        <tr class="horizontal-offset-setting">
          <td>水平方向のオフセット[px]</td>
          <td><input type="number" name="horizontal-offset" value="2" min="-1000" max="1000"/></td>
        </tr>
        <tr class="vertical-offset-setting">
          <td>垂直方向のオフセット[px]</td>
          <td><input type="number" name="vertical-offset" value="2" min="-1000" max="1000"/></td>
        </tr>
        <tr class="blur-setting">
          <td>ぼかしの距離[px] (0～)</td>
          <td><input type="number" name="blur" value="2" min="0" max="1000"/></td>
        </tr>
        <tr class="spreading-setting">
          <td>影の拡がり[px]</td>
          <td><input type="number" name="spreading" value="2" min="-1000" max="1000"/></td>
        </tr>
        <tr class="shadow-color-setting">
          <td>影の色</td>
          <td>
            <input type="color" name="shadow-color" />
          </td>
        </tr>
        <tr class="background-color-setting">
          <td>背景色</td>
          <td>
            <input type="color" name="background-color" />
          </td>
        </tr>
      </tbody>
    </table>
    <div class="shadow-image">
      <div class="image-container">
        <div class="shadow-object"></div>
      </div>
    </div>
    <div class="sample-code">
      <textarea></textarea>
    </div>
  </div>
</template>

<script>
export default {
  name: "app"
};
</script>

<style lang="scss" scoped>
#app {
  .shadow-settings {
    .horizontal-offset-setting {
    }

    .vertical-offset-setting {
    }

    .blur-setting {
    }

    .spreading-setting {
    }

    .shadow-color-setting {
    }

    .background-color-setting {

    }
  }

  .shadow-image {
    .image-container {
      background-color: white;
      border: 1px gray solid;

      .shadow-object {
        width: 100px;
        height: 100px;
        margin: 150px;
        background-color: gray;
        box-shadow: 2px 2px 2px 2px rgba(0, 0, 0, 0.4);
      }
    }
  }

  .sample-code {
  }
}
</style>
