<template>
    <div class="container">
        <div class="row mt-5">
            <div class="col-md-12">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Data Warga</h3>
                        <div class="card-tools">
                            <button
                                class="btn btn-success"
                                data-toggle="modal"
                                data-target="#addNew"
                            >
                                Tambah <i class="fas fa-user-plus fa-fw"></i>
                            </button>
                        </div>
                    </div>

                    <div class="card-body table-responsive p-0">
                        <table class="table table-hover text-nowrap">
                            <thead>
                                <tr>
                                    <th>ID</th>
                                    <th>Nama</th>
                                    <th>Usia</th>
                                    <th>Jenis Kelamin</th>
                                    <th>Pendidikan Terakhir</th>
                                    <th>Alamat Lengkap</th>
                                    <th>Pekerjaan</th>
                                    <th>Penghasilan</th>
                                    <th>Tingkat kerusakan</th>
                                    <th></th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>1</td>
                                    <td>John Doe</td>
                                    <td>35 Tahun</td>
                                    <td>Laki-Laki</td>
                                    <td>SMA</td>
                                    <td>Paruga Nae</td>
                                    <td>Wiraswasta</td>
                                    <td>Rp.1.500.000</td>
                                    <td>80%</td>
                                    <td>
                                        <a href="#">
                                            <i
                                                class="fa fa-edit btn btn-warning"
                                            ></i>
                                        </a>

                                        /
                                        <a href="#">
                                            <i
                                                class="fa fa-trash btn btn-danger"
                                            ></i>
                                        </a>
                                    </td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </div>
        <!-- Modal -->
        <div class="modal" tabindex="-1" id="addNew" aria-labelledby="addNewLabel"
            aria-hidden="true">
            <div class="modal-dialog modal-dialog-centered">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title" id="addNewLabel">Tambahkan Data Warga</h5>
                        <button  type="button"
                            class="close"
                            data-dismiss="modal"
                            aria-label="Close">
                         <span aria-hidden="true">&times;</span>
                        </button>
                    </div>
                    <div class="modal-body">
                        <div class="form-grup">

                        </div>
                    </div>
                    <div class="modal-footer">
                        <button
                            type="button"
                            class="btn btn-danger"
                            data-bs-dismiss="modal"
                        >
                            Close
                        </button>
                        <button type="button" class="btn btn-primary">
                            Save changes
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            form: new Form({
                name: "",
                password: "",
            }),
        };
    },
    mounted() {
        console.log("Component mounted.");
    },
};
</script>
