<template>
  <form action="#" class="mb-3">
    <fieldset>
      <input name="input-text" type="text" class="mr-1" />
      <button class="mr-1">Click</button>
      <span>123</span>
    </fieldset>

    <fieldset>
      <select name="input-select" class="mr-1">
        <option value="1">value 1</option>
        <option value="2">value 2</option>
        <option value="3">value 3</option>
        <option value="4">value 4</option>
      </select>
      <button class="mr-1">Click</button>
      <span>123</span>
    </fieldset>

    <fieldset>
      <input name="input-checkbox" id="checkbox" type="checkbox" class="mr-1" />
      <label class="mr-1" for="checkbox">checkbox</label>
      <button class="mr-1">Click</button>
      <span>123</span>
    </fieldset>

    <fieldset>
      <div>
        <input name="input-radio" id="radio-1" type="radio" class="mr-1" value="1" />
        <label class="mr-1" for="radio-1">radio-1</label>
      </div>

      <div>
        <input name="input-radio" id="radio-2" type="radio" class="mr-1" value="2" />
        <label class="mr-1" for="radio-2">radio-2</label>
      </div>

      <div class="mb-1">
        <input name="input-radio" id="radio-3" type="radio" class="mr-1" value="3" />
        <label class="mr-1" for="radio-3">radio-3</label>
      </div>

      <button class="mr-1">Click</button>
      <span>123</span>
    </fieldset>

    <button>Submit</button>
  </form>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
fieldset {
  margin-bottom: 10px;
}
</style>