<template>
    <!-- Carrusel -->
    <div class="row justify-content-center">
        <div class="col-md-6">
            <div class="card mt-4 mb-4">
                <div class="card-body text-center">
                    <h5 class="card-title">Galería de Automóviles</h5>
                    <div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
                        <div class="carousel-inner">
                            <div class="carousel-item active">
                                <img src="https://imgs.search.brave.com/9LhnGCNWmq4Zb_If-L_Wfxa-i5T0yD1k0z4NtHJ3qtI/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tZWRp/YS5pc3RvY2twaG90/by5jb20vaWQvMTM1/MzA3NjQ1NS9lcy9m/b3RvLzE5Njctc2hl/bGJ5LWNvYnJhLWd0/NTAwLWZhc3RiYWNr/LWNvdXAlQzMlQTku/anBnP3M9NjEyeDYx/MiZ3PTAmaz0yMCZj/PUs1WFp6Z3FMOFBS/cmVXUHZST21SSjY5/TWhSaThwVmw1U0ZN/aUVEVGM5Y0E9" class="d-block w-100" alt="Carro 1">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/a1qLFmINRGNhvNRlKw-YNQp3Zt79Y-a3wSt7g3CNrZ0/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly91cGxv/YWQud2lraW1lZGlh/Lm9yZy93aWtpcGVk/aWEvY29tbW9ucy82/LzY1LzE5NjhfQ2Ft/YXJvX1JTXzMyNy5q/cGc" class="d-block w-100" alt="Carro 2">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/52gvmX9Wnz6oUQuxSuakU6DD93Qz5bgjm7Vj4U87kEc/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tZWRp/YS5nZXR0eWltYWdl/cy5jb20vaWQvNDg3/NzM5ODA4L2VzL2Zv/dG8vZXN0YWRvdW5p/ZGVuc2UtY2wlQzMl/QTFzaWNhLWF1dG9t/JUMzJUIzdmlsLTE5/NTgtY2hldnJvbGV0/LWNvcnZldHRlLWMx/LmpwZz9zPTYxMng2/MTImdz0wJms9MjAm/Yz1iZUphbVRJamVF/RE5LUlR6V1E4T2pv/SkJ2VDNDZFVaLXp3/aXU2UXA2VWtnPQ" class="d-block w-100" alt="Carro 3">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/9kJHAceiHULMfZpXGYSxSNu4pw8FHmpnEXWxjOP7-3I/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tbGlu/LmVzL3dwLWNvbnRl/bnQvdXBsb2Fkcy8y/MDI0LzA4L0ZvcmQt/R1QtMjAwNS5qcGVn" class="d-block w-100" alt="Carro 3">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/NcPPzTi5KWx81FE-I5kWGPX1TublRM2fwyncX5qatH0/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tbGlu/LmVzL3dwLWNvbnRl/bnQvdXBsb2Fkcy8y/MDI0LzA4L0RvZGdl/LUNoYXJnZXItRGF5/dG9uYS0xOTY5LTEw/MjR4NjgzLmpwZw" class="d-block w-100" alt="Carro 3">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/ydMyfQLASWyw_mJP8W9BHM3_KguW9OujUuKAtIY206A/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tZWRp/YS5nZXR0eWltYWdl/cy5jb20vaWQvMTMy/NDIxMzU4NS9lcy9m/b3RvL3ZvbHZvLTE4/MDAtY2wlQzMlQTFz/aWNvLWVuLXVuYS1w/aXN0YS1hcmJvbGFk/YS5qcGc_cz02MTJ4/NjEyJnc9MCZrPTIw/JmM9NzlmRXYyOTEx/ckowdm9neDJabFVJ/UG9EV1dsZlFDOHFG/blg1ZDhGcWU4VT0" class="d-block w-100" alt="Carro 3">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/S0Oo5MuvsCedyHpnSdyWj-_Xmoz0iQF70sz9hHXzOWY/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly93d3cu/Z2FsdmFubGFjYWRv/cy5jb20vd3AtY29u/dGVudC91cGxvYWRz/LzIwMTgvMDUvUG9y/c2NoZV85MTEuanBn" class="d-block w-100" alt="Carro 3">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/lDOrCI1AUoZ1cpf1cxbMoAmohO70Oin8V9tfTSqH5fo/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tZWRp/YS5nZXR0eWltYWdl/cy5jb20vaWQvNDU5/MjYxOTA5L2VzL2Zv/dG8vZm9yZC1tdXN0/YW5nLmpwZz9zPTYx/Mng2MTImdz0wJms9/MjAmYz1Ub3Q0Rk5M/ZnlKNmI0cDUwelA2/NXBhbENWVTRZWm5t/d1FwUmVYbngyaWdR/PQ" class="d-block w-100" alt="Carro 3">
                            </div>
                            <div class="carousel-item">
                                <img src="https://imgs.search.brave.com/mv2qyb0ML3bDnDYOAf81HxXfffQETN0qo3dJU0bW8zc/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9tZWRp/YS5pc3RvY2twaG90/by5jb20vaWQvMTM0/MDc1NDc3MS9lcy9m/b3RvLzE5NjgtZm9y/ZC1zaGVsYnktY29i/cmEtbXVzdGFuZy1n/dDUwMC1mYXN0YmFj/ay5qcGc_cz02MTJ4/NjEyJnc9MCZrPTIw/JmM9M2U5Mkx3QWFp/eUs2UHFjM2ZiamJY/dDBxcUJxNFY0STd2/Q01vcDdSNEQ2Yz0" class="d-block w-100" alt="Carro 3">
                            </div>
                        </div>
                        
                        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample"
                            data-bs-slide="prev">
                            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Anterior</span>
                        </button>
                        <button class="carousel-control-next" type="button" data-bs-target="#carouselExample"
                            data-bs-slide="next">
                            <span class="carousel-control-next-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Siguiente</span>
                        </button>
                    </div>
                    <p class="mt-2">Explora nuestra colección de automóviles clasicos</p>
                    <a href="#" class="btn btn-warning">Más información</a>
                </div>
            </div>
        </div>
    </div>
    
</template>