<template>
    <div class="w-full">
        <IbeRoom :room=this.room1></IbeRoom>
        <IbeRoom :room=this.room2></IbeRoom>
        <IbeRoom :room=this.room3></IbeRoom>

    </div>
</template>

<script>
    import IbeRoom from "./IbeRoom";
    export default {
        components: {
            IbeRoom
        },
        data: function() {
            return {
                room1: {
                    code: "STD",
                    title: "Standard Room",
                    summary: "Studio Apartment with an area of 41 m2. Max cap.: 2 adults + 1 child up to 2 years old",
                    card_amenities: [
                        {
                            label: "Sleeps",
                            value: 3
                        },
                        {
                            label: "Beds",
                            value: "2 Twin"
                        },
                        {
                            label: "Area",
                            value: "41 m²"
                        },
                    ],
                    image: "background-image: url('/uploads/rooms/room-0.jpg')",
                    rates: [
                        {
                            code: "BAR",
                            title: "Best Available Rate",
                            summary: "Hotel's Best Available Rate. Accommodation and all taxes included.",
                            from: 190
                        },
                        {
                            code: "NFR",
                            title: "Non Refundable",
                            summary: "Hotel's Non Refundable Rate. Accommodation and all taxes included.",
                            from: 155
                        }
                    ]
                },
            room2: {
                code: "DBL",
                title: "Double Room",
                summary: "Studio Apartment with an area of 41 m2. Max cap.: 2 adults + 1 child up to 2 years old",
                card_amenities: [
                    {
                        label: "Sleeps",
                        value: 2
                    },
                    {
                        label: "Beds",
                        value: "1 Twin"
                    },
                    {
                        label: "Area",
                        value: "21 m²"
                    },
                ],
                image: "background-image: url('/uploads/rooms/room-1.jpg')",
                rates: [
                    {
                        code: "BAR",
                        title: "Best Available Rate",
                        summary: "Hotel's Best Available Rate. Accommodation and all taxes included.",
                        from: 120
                    },
                    {
                        code: "NFR",
                        title: "Non Refundable",
                        summary: "Hotel's Non Refundable Rate. Accommodation and all taxes included.",
                        from: 115
                    }
                ]
            },
            room3: {
                code: "ST",
                title: "Suite",
                summary: "Studio Apartment with an area of 41 m2. Max cap.: 2 adults + 1 child up to 2 years old",
                card_amenities: [
                    {
                        label: "Sleeps",
                        value: 4
                    },
                    {
                        label: "Beds",
                        value: "2 Twin"
                    },
                    {
                        label: "Area",
                        value: "61 m²"
                    },
                ],
                image: "background-image: url('/uploads/rooms/room-2.jpg')",
                rates: [
                    {
                        code: "BAR",
                        title: "Best Available Rate",
                        summary: "Hotel's Best Available Rate. Accommodation and all taxes included.",
                        from: 170
                    },
                    {
                        code: "NRF",
                        title: "Non Refundable",
                        summary: "Hotel's Non Refundable Rate. Accommodation and all taxes included.",
                        from: 175
                    }
                ]
            }
        }
    },
        name: 'IbeRoomList',
        props: {

        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
