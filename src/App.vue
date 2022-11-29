<script>
export default {
  data: function () {
    return {
      darkMode: false,
    };
  },
  dark() {
    document.querySelector("body").classList.add("dark-mode");
    this.darkMode = true;
    this.$emit("dark");
  },
  light() {
    document.querySelector("body").classList.remove("dark-mode");
    this.darkMode = false;
    this.$emit("light");
  },
  modeToggle() {
    if (
      this.darkMode ||
      document.querySelector("body").classList.contains("dark-mode")
    ) {
      this.light();
    } else {
      this.dark();
    }
  },
  computed: {
    darkDark() {
      return this.darkMode && "darkmode-toggled";
    },
  },
};
</script>

<template>
  <div class="container text-center">
    <div class="row">
      <div class="col">
        <img
          src="https://www.dictionary.com/e/wp-content/uploads/2018/03/rickrolling-300x300.jpg"
          class="img-thumbnail"
          alt="..."
        />
      </div>
      <div class="col-6">
        <h3>Edit User</h3>
        <button type="button" class="btn btn-outline-primary">
          Submit Changes
        </button>
        <h6>Light</h6>
        <label class="switch">
          <input type="checkbox" onchange="darkMode()" />
          <span class="slider round"></span>
        </label>
        <h6>Dark</h6>
      </div>
      <div class="col">Re-Connect Linkedin Profile</div>
      <div class="row">
        <div class="col">
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
            <label for="formGroupExampleInput" class="form-label"
              >Password</label
            >
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
          <h5>Alert Types</h5>
          <button type="button" class="btn btn-outline-primary">Tasks</button>
          <button type="button" class="btn btn-outline-primary">
            Appointments
          </button>
          <button type="button" class="btn btn-outline-primary">Notex</button>
          <button type="button" class="btn btn-outline-primary">Leads</button>
          <button
            type="button"
            class="btn btn-outline-primary"
            style="width: 33%"
          >
            Candidates
          </button>
          <button
            type="button"
            class="btn btn-outline-primary"
            style="width: 33%"
          >
            Contacts
          </button>
          <button
            type="button"
            class="btn btn-outline-primary"
            style="width: 33%"
          >
            Companies
          </button>
          <button
            type="button"
            class="btn btn-outline-primary"
            style="width: 100%"
          >
            Submissions
          </button>
          <h5>Delivery Methods</h5>
          <button
            type="button"
            class="btn btn-outline-primary"
            style="width: 50%"
          >
            Email
          </button>
          <button
            type="button"
            class="btn btn-outline-primary"
            style="width: 50%"
          >
            Slack
          </button>
          <div class-name="last-options">
            <p>SMS (contact us to enable this method)</p>
            <br />
            <p>MS Teams (contact us to enable this method)</p>
            <br />
            <p>Zoom (contact us to enable this method)</p>
            <br />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.mb-3 {
  text-align: left;
}
h5 {
  text-align: left;
}
p {
  text-align: left;
}
.container {
  padding-top: 100px;
}
</style>
