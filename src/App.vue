<script></script>
<template>
  <div class="container text-center">
    <div class="row">
      <div class="col">1 of 3</div>
      <div class="col-6">
        2 of 3 (wider)
        <h3>Edit User</h3>
        <button type="button" class="btn btn-outline-primary">Primary</button>
      </div>

      <div class="col">3 of 3</div>
    </div>
    <div class="row">
      <div class="col">
        1 of 3
        <div class="mb-3">
          <label
            type="text"
            for="formGroupExampleInput"
            class="form-label"
            style="align-content: left"
            >First Name</label
          >
          <input
            type="text"
            class="form-control"
            id="formGroupExampleInput"
            placeholder="First Name"
          />
        </div>
        <div class="mb-3">
          <label for="formGroupExampleInput2" class="form-label"
            >Last Name</label
          >
          <input
            type="text"
            class="form-control"
            id="formGroupExampleInput2"
            placeholder="Last Name"
          />
        </div>
        <div class="mb-3">
          <label for="formGroupExampleInput" class="form-label">Title</label>
          <input
            type="text"
            class="form-control"
            id="formGroupExampleInput"
            placeholder="Title"
          />
        </div>
        <div class="mb-3">
          <label for="formGroupExampleInput2" class="form-label">Role</label>
          <input
            type="text"
            class="form-control"
            id="formGroupExampleInput2"
            placeholder="Role"
          />
        </div>
      </div>
      <div class="col">
        2 of 3 (wider)
        <div class="mb-3">
          <label for="formGroupExampleInput" class="form-label">Email</label>
          <input
            type="email"
            class="form-control"
            id="Email"
            placeholder="Enter a valid Email"
          />
        </div>
        <div class="mb-3">
          <label for="formGroupExampleInput2" class="form-label">Phone</label>
          <input
            type="phone"
            class="form-control"
            id="Phone"
            placeholder="Enter phone"
          />
        </div>
        <div class="mb-3">
          <label for="formGroupExampleInput" class="form-label">Password</label>
          <input
            type="password"
            class="form-control"
            id="Password"
            placeholder="Enter your password"
          />
        </div>
        <div class="mb-3">
          <label for="formGroupExampleInput2" class="form-label"
            >Default Note Action</label
          >
          <input
            type="text"
            class="form-control"
            id="Default Note Action"
            placeholder="Client Submission"
          />
        </div>
        <div class="mb-3">
          <label for="formGroupExampleInput2" class="form-label"
            >Default Landing Page upon Login</label
          >
          <input
            type="text"
            class="form-control"
            id="Default Landiing Page upon Login"
            placeholder="Dashboard"
          />
        </div>
      </div>
      <div class="col">
        3 of 3
        <h5>Alert Types</h5>
        <button type="button" class="btn btn-outline-primary">Primary</button>
        <button type="button" class="btn btn-outline-primary">Primary</button>
        <button type="button" class="btn btn-outline-primary">Primary</button>
        <button type="button" class="btn btn-outline-primary">Primary</button>
        <button
          type="button"
          class="btn btn-outline-primary"
          style="width: 33%"
        >
          Primary
        </button>
        <button
          type="button"
          class="btn btn-outline-primary"
          style="width: 33%"
        >
          Primary
        </button>
        <button
          type="button"
          class="btn btn-outline-primary"
          style="width: 33%"
        >
          Primary
        </button>
        <button
          type="button"
          class="btn btn-outline-primary"
          style="width: 100%"
        >
          Primary
        </button>
        <h5>Delivery Methods</h5>
        <button
          type="button"
          class="btn btn-outline-primary"
          style="width: 50%"
        >
          Primary
        </button>
        <button
          type="button"
          class="btn btn-outline-primary"
          style="width: 50%"
        >
          Primary
        </button>
        <p>SMS (contact us to enable this method)</p>
        <p>MS Teams (contact us to enable this method)</p>
        <p>Zoom (contact us to enable this method)</p>
      </div>
    </div>
  </div>
</template>

<style>
.mb-3 {
  text-align: left;
}
</style>
