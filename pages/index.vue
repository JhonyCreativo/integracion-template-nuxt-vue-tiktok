<template>
    <AdminTemplate>
        <div class="card">
            <div class="card-header border-bottom">
                <h5 class="card-title mb-3">Tareas</h5>
            </div>
            <div class="card-datatable table-responsive">
                <div class="dataTables_wrapper dt-bootstrap5 no-footer">
                    <div class="row me-2">

                        <div class="col-md-12">
                            <div
                                class="dt-action-buttons text-xl-end text-lg-start text-md-end text-start d-flex align-items-center justify-content-end flex-md-row flex-column mb-3 mb-md-0">

                                <div class="dt-buttons btn-group flex-wrap my-4">
                                    <button class="btn btn-secondary add-new btn-primary" type="button" data-bs-toggle="modal" data-bs-target="#modalTask">
                                        <span>
                                            <i class="ti ti-plus me-0 me-sm-1 ti-xs"></i>
                                            <span class="d-none d-sm-inline-block">Agregar</span>
                                        </span>
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <table class="datatables-users table dataTable no-footer dtr-column">
                        <thead class="border-top">
                            <tr class="bg-dark">
                                <th class="text-white">#</th>
                                <th class="text-white">Descripcion</th>
                                <th class="text-white">Accion</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>1</td>
                                <td>Descripcion de la tarea</td>
                                <td>
                                    <div class="btn-group">
                                        <button class="btn btn-sm btn-info"><i class="ti ti-pencil"></i></button>
                                        <button class="btn btn-sm btn-danger"><i class="ti ti-trash"></i></button>
                                    </div>
                                </td>
                            </tr>
                        </tbody>
                    </table>

                </div>
            </div>
            <div class="modal fade " id="modalTask" tabindex="-1"  aria-modal="true" role="dialog">
                <div class="modal-dialog modal-md modal-simple modal-edit-user">
                    <div class="modal-content">
                        <div class="modal-body">
                            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                            <div class="text-center mb-4">
                                <h3 class="mb-2">Tarea</h3>           
                            </div>
                            <form id="modalTaskForm" class="row g-3 fv-plugins-bootstrap5 fv-plugins-framework"
                                onsubmit="return false" novalidate="novalidate">
                                <div class="col-12 text-left">
                                    <label class="form-label" for="modalmodalTaskName">Descripcion</label>
                                    <input type="text"  class="form-control"> 
                                </div>
                                <div class="col-12 text-center">
                                    <button type="reset" class="btn btn-label-secondary waves-effect" data-bs-dismiss="modal" aria-label="Close">
                                        Cancelar
                                    </button>
                                    <button type="submit" class="btn btn-success me-sm-3 mx-2 waves-effect waves-light">Guardar</button>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </AdminTemplate></template>

<script>
export default {
    name: 'IndexPage',
}
</script>