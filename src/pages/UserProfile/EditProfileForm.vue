<template>
  <card>
    <h4 slot="header" class="card-title">Mi Perfil</h4>
    <form>
      <div class="row">
        <div class="col-md-5">
          <base-input type="text"
                    label="Codigo"
                    :disabled="true"
                    placeholder="codigo"
                    v-model="user.company">
          </base-input>
        </div>

        <div class="col-md-5">
          <base-input type="text"
                    label="Nombre"
                    placeholder="Nombre"
                    v-model="user.username">
          </base-input>
        </div>
        
      </div>

      <div class="row">
        <div class="col-md-6">
          <base-input type="text"
                    label="Apellido Paterno"
                    placeholder="Apellido Paterno"
                    v-model="user.firstName">
          </base-input>
        </div>
        <div class="col-md-6">
          <base-input type="text"
                    label="Apellido Materno"
                    placeholder="Apellido Materno"
                    v-model="user.lastName">
          </base-input>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <base-input type="text"
                    label="Address"
                    placeholder="Home Address"
                    v-model="user.address">
          </base-input>
        </div>
      </div>

      <div class="row">
        <div class="col-md-4">
          <base-input type="text"
                    label="City"
                    placeholder="City"
                    v-model="user.city">
          </base-input>
        </div>
        <div class="col-md-4">
          <base-input type="text"
                    label="Country"
                    placeholder="Country"
                    v-model="user.country">
          </base-input>
        </div>
        <div class="col-md-4">
          <base-input type="number"
                    label="Postal Code"
                    placeholder="ZIP Code"
                    v-model="user.postalCode">
          </base-input>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <div class="form-group">
            <label>About Me</label>
            <textarea rows="5" class="form-control border-input"
                      placeholder="Here can be your description"
                      v-model="user.aboutMe">
              </textarea>
          </div>
        </div>
      </div>
      <div class="text-center">
        <button type="submit" class="btn btn-info btn-fill float-right" @click.prevent="updateProfile">
          Update Profile
        </button>
      </div>
      <div class="clearfix"></div>
    </form>
  </card>
</template>
<script>

  export default {
    
    data () {
      return {
        user: {
        }
      }
    },
    
  }

</script>
<style>

</style>
