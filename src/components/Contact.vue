<template>
    <section id="contact" class="bg-primary py-5">
        <div class="container">
            <app-title title-value="contact" subtitle-value="Lorem ipsum dolor sit amet." color="light"></app-title>
            <div class="row mt-5">
                <div class="col-md-6 mb-3">
                    <div class="card">
                        <div class="card-body">
                            <div class="card-title mb-4">
                                <h4 class="text-secondary text-capitalize mb-1">contact us</h4>
                                <p>If you’d like to hire us, or just shoot the breeze, please fill in the form below.</p>
                            </div>
                            <form action="">
                                <div class="form-group">
                                <input type="text" placeholder="Name*" name="name" id="name" class="form-control my-3">
                                <input type="text" placeholder="Email*" name="email" id="email" class="form-control my-3">
                                <textarea placeholder="Message*" name="message" id="message" class="form-control my-3"></textarea>
                                <button id="send-message" class="btn mt-5 btn-lg btn-warning text-uppercase btn-block">send</button>
                                </div>
                                
                            </form>

                        </div>
                    </div>
                </div>
                <div class="col-md-6 mb-3 align-self-center">
                    <div class="embed-responsive embed-responsive-4by3">
                        <iframe  class="embed-responsive-item" :src="map" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data () {
        return {
            map: "https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d26764.815934994243!2d35.25579634463031!3d33.014267213960686!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x151c2db7457142f1%3A0xde4160c0ab1b47c1!2sMaalot-Tarshiha!5e0!3m2!1sen!2sil!4v1526923217026"
        }
    }
}
</script>
