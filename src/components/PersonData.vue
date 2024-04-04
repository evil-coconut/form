<template>
    <div class="container">
        <InputText labelName="Имя"/>
        <InputText labelName="Фамилия"/>
        <InputText labelName="Отчество"/>
        <InputData labelName="Дата рождения"/>
        <InputNumber labelName="Номер телефона"/>
        <div>
            <label for="female">
                <input type="radio" id="female" value="Женский" name="gender"/>
                Женский
            </label>
            <label for="male">
                <input type="radio" id="male" value="Мужской" name="gender"/>
                Мужской
            </label>
        </div>
        <List labelName="Группа клиентов" :listItems='groupClients'/>
        <List labelName="Лечащий врач" :listItems='groupDoctors'/>
        <label for="sms">
            <input type="checkbox" id="sms"/>
            Не отправлять СМС.
        </label>
    </div>
</template>

<script setup>
    import InputText from "./input/InputText.vue";
    import InputNumber from "./input/InputNumber.vue";
    import InputData from "./input/InputData.vue";
    import List from "./list/List.vue"

    const groupClients = ['VIP', 'Проблемные', 'ОМС'];
    const groupDoctors = ['Иванов', 'Захаров', 'Чернышева'];
</script>

<style scoped>
.container {
    display: flex;
    flex-direction: column;
    gap: 10px;
}
</style>