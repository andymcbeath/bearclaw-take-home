<script>
export default {
  data: function () {
    return {
      darkMode: false,
      checked: true,
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
  <div class="container">
    <div class="row">
      <div class="col">
        <div class="picture">
          <img
            src="@/assets/never-gonna-give.png"
            class="img-thumbnail"
            alt="..."
          />
        </div>
      </div>
      <div class="col-6">
        <div class="edit-user">
          <h1>Edit User</h1>
        </div>
        <br />
        <div class="middle-top">
          <button type="button" class="btn btn-outline-primary">
            Submit Changes
          </button>
          <h6>LIGHT</h6>
          <label class="switch">
            <input type="checkbox" onchange="darkMode()" />
            <span class="slider round"></span>
          </label>
          <h6>DARK</h6>
          <h6>STABLE</h6>
          <label class="switch">
            <input type="checkbox" @click="toggleCheckbox" />
            <div class="slider round"></div>
          </label>
          <h6>BETA</h6>
        </div>
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
        <div id="buttons" class="col">
          <div class="d-grid gap-2 d-md-block">
            <h5>Alert Types</h5>
            <button type="button" class="btn btn-outline-primary">Tasks</button>
            <button type="button" class="btn btn-outline-primary">
              Appointments
            </button>
            <button type="button" class="btn btn-outline-primary">Notes</button>
            <button type="button" class="btn btn-outline-primary">Leads</button>
            <button type="button" class="btn btn-outline-primary">
              Candidates
            </button>
            <button type="button" class="btn btn-outline-primary">
              Contacts
            </button>
            <button type="button" class="btn btn-outline-primary">
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
          </div>
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
.toggle-seperator {
  padding-left: 4%;
  padding-right: 1%;
}
.edit-user {
  font-size: xx-large;
}
.mb-3 {
  text-align: left;
}
h5 {
  text-align: left;
}
p {
  text-align: left;
  color: white;
}
.container {
  padding-top: 100px;
}
.middle-top {
  display: flex;
}
h6 {
  padding-left: 2%;
}
img.img-thumbnail {
  border-color: rgba(0, 0, 0, 0.847);
  border-radius: 50%;
  width: 150px;
  height: 150px;
  border-width: 15px;
  color: rgba(0, 0, 0, 0.847);
}
.picture {
  color: black;
  background-color: black;
  border-color: rgba(0, 0, 0, 0.847);
  color: rgba(0, 0, 0, 0.847);
  border-radius: 50%;
  width: 150px;
  height: 150px;
}
</style>
