<script lang="ts">
  function setIndeterminate(node: HTMLInputElement) {
    node.indeterminate = true;
  }
</script>

<div class="m-2">
  <div class="my-2">
    <input type="range" class="form-range" />
  </div>
  <div class="my-2">
    <select class="form-select">
      <option>Test 1</option>
      <option>Test 2</option>
      <option>Test 3</option>
      <option>Test 4</option>
      <option>Test 5</option>
    </select>
    <select class="form-select" disabled>
      <option>Test 1</option>
      <option>Test 2</option>
      <option>Test 3</option>
      <option>Test 4</option>
      <option>Test 5</option>
    </select>
    <select class="form-select sm">
      <option>Test 1</option>
      <option>Test 2</option>
      <option>Test 3</option>
      <option>Test 4</option>
      <option>Test 5</option>
    </select>
    <select class="form-select lg">
      <option>Test 1</option>
      <option>Test 2</option>
      <option>Test 3</option>
      <option>Test 4</option>
      <option>Test 5</option>
    </select>
  </div>
  <div class="flex gap-3 my-2">
    <label>
      <input class="form-checkbox" type="checkbox" checked /> Checkbox
    </label>
    <label>
      <input class="form-checkbox" type="checkbox" checked disabled /> Checkbox
    </label>
    <label>
      <input class="form-checkbox" type="checkbox" disabled /> Checkbox
    </label>
    <label>
      <input class="form-checkbox" type="checkbox" use:setIndeterminate /> Checkbox
    </label>
  </div>
  <div class="flex gap-3 my-2">
    <label>
      <input class="form-check-input" type="checkbox" checked /> Checkbox Bootstrap
    </label>
    <label>
      <input class="form-check-input" type="checkbox" /> Checkbox Bootstrap
    </label>
  </div>
  <div class="flex gap-3 my-2">
    <label>
      <input class="form-radio" type="radio" name="test-radio" checked /> Radio
    </label>
    <label>
      <input class="form-radio" type="radio" name="test-radio" /> Radio
    </label>
  </div>
  <div class="flex gap-1 my-2">
    <input class="form-input lg border-rose-500" type="email" placeholder="Enter email" />
    <input class="form-input lg border-rose-500 min-w-[5rem]" type="color" />
  </div>
  <input class="form-input block" type="email" placeholder="Enter email" value="test@mail.ru" />
  <input
    class="form-input block"
    type="email"
    placeholder="Enter email"
    value="test@mail.ru: disabled"
    disabled
  />
  <div>
    <input
      class="form-input"
      type="email"
      placeholder="Enter email"
      value="test@mail.ru"
      readonly
    />
    <input class="form-input" type="color" value="#ff0011" />
  </div>
  <div>
    <input class="form-input" type="date" value="2023-01-23" />
    <input class="form-input" type="datetime" value="2023-01-23T12:23" />
    <input class="form-input" type="datetime-local" value="2023-01-23T21:23" />
  </div>
  <input class="form-input" type="number" />
  <div>
    <input class="form-input" type="password" placeholder="Enter password" />
    <input class="form-input" type="password" value="1234" />
  </div>
  <div>
    <input class="form-input" type="search" placeholder="Search" />
    <input class="form-input" type="search" value="1234" />
    <input class="form-input" type="text" placeholder="Text" />
    <input class="form-input" type="tel" value="+1234" />
  </div>
  <div>
    <input class="form-input" type="month" />
    <input class="form-input" type="time" />
    <input class="form-input" type="week" placeholder="Week" />
    <input class="form-input" type="url" />
  </div>
  <div class="my-3">
    <input class="form-button" type="button" value="Submit" />
    <button class="form-button" disabled>Test</button>
    <button class="form-button">Test</button>
    <button class="form-button" disabled>TestD</button>
  </div>
  <div class="my-3">
    <input class="form-button sm" type="button" value="Submit" />
    <button class="form-button sm" disabled>Test</button>
    <button class="form-button sm">Test</button>
    <button class="form-button sm" disabled>TestD</button>
  </div>
  <div class="my-3">
    <input class="form-button primary sm" type="button" value="Submit" />
    <button class="form-button primary sm" disabled>Test</button>
    <button class="form-button primary sm">Test</button>
    <button class="form-button primary sm" disabled>TestD</button>
  </div>
  <div class="my-3">
    <input class="form-input" type="file" />
    <input class="form-input sm" type="file" />
    <input class="form-input lg" type="file" />
  </div>
  <div class="flex justify-center">
    <div class="mb-3 w-96">
      <label for="formFile" class="form-label inline-block mb-2 text-gray-700"
        >Default file input example</label
      >
      <input
        class="form-control
    block
    w-full
    px-3
    py-1.5
    text-base
    font-normal
    text-gray-700
    bg-white bg-clip-padding
    border border-solid border-gray-300
    rounded
    transition
    ease-in-out
    m-0
    focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none"
        type="file"
        id="formFile"
      />
    </div>
  </div>
</div>
