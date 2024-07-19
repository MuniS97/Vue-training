<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <main>
    <h1>Калькулятор</h1>
    <div class="first-div">
      <h2>Расчёт процента жира</h2>
      <form class="first-div-form">
        <div class="form-first-div">
          <div>
            <label for="waist">Талия</label>
            <input type="text" id="waist" placeholder="Заполните поле" />
          </div>
          <div>
            <label for="neck">Шея</label>
            <input type="text" id="neck" placeholder="Заполните поле" />
          </div>
          <div>
            <label for="height">Рост</label>
            <input type="text" id="height" placeholder="Заполните поле" />
          </div>
          <div>
            <label for="hips">Бёдра</label>
            <input type="text" id="hips" placeholder="Заполните поле" />
          </div>
        </div>
        <div class="form-second-div">
          <div>
            <label for="fat">% жира</label>
            <input type="text" id="fat" placeholder="00" />
          </div>
          <button type="submit">Рекомендации</button>
        </div>
      </form>
    </div>
    <div class="second-div">
      <h2>Расчёт процента жира</h2>
      <form class="second-div-form">
        <div class="form-first-div">
          <div class="form-first-div-first-div">
            <div>
              <label for="weight">Вес (кг)</label>
              <input type="text" id="weight" placeholder="Заполните поле" />
            </div>
            <div>
              <label for="activity">Коэффициент активности</label>
              <input type="text" id="activity" placeholder="Заполните поле" />
            </div>
          </div>
          <div class="form-first-div-last-div">
            <p>1,2 — сидячий образ жизни, минимум движений</p>
            <p>1,3 — малоподвижный образ жизни, 3–5 тыс. шагов в день</p>
            <p>1,4 — умеренная активность, 8–10 тыс. шагов в день</p>
            <p>1,5 — активный образ жизни, 12–15 тыс. шагов в день</p>
          </div>
        </div>
        <div class="form-second-div">
          <div>
            <p>
              Масса тела <br />
              без жира
            </p>
            <h4>58 <span>кг</span></h4>
          </div>
          <div>
            <p>
              Обмен веществ <br />
              в покое
            </p>
            <h4>1406 <span>Ккал</span></h4>
          </div>
          <div>
            <p>
              Расход калорий <br />
              в сутки
            </p>
            <h4>1828 <span>Ккал</span></h4>
          </div>
        </div>
      </form>
    </div>
    <div class="third-div">
      <h2>Третий подзаголовок</h2>
      <div class="third-div-first-div">
        <form class="third-div-form">
          <div>
            <label for="dailynorm">Суточная норма Ккал</label>
            <input type="text" id="dailynorm" placeholder="Заполните поле" />
          </div>
          <div>
            <label for="protein">Белки</label>
            <input type="text" id="protein" placeholder="Заполните поле" />
          </div>
          <div>
            <label for="fats">Жиры</label>
            <input type="text" id="fats" placeholder="Заполните поле" />
          </div>
          <div>
            <label for="carbohydrates">Углеводы</label>
            <input type="text" id="carbohydrates" placeholder="Заполните поле" />
          </div>
        </form>
        <div>
          <div class="third-div-min-first">
            <h3>Суточная норма в граммах</h3>
            <div>
              <p>Белки <span>192</span></p>
              <p>Жиры <span>77</span></p>
              <p>Углеводы <span>100</span></p>
              <p>Ккал <span>1900</span></p>
            </div>
          </div>
          <div class="third-div-min-second">
            <h3>Всего за сегодня</h3>
            <div>
              <p>Белки <span>00</span></p>
              <p>Жиры <span>00</span></p>
              <p>Углеводы <span>00</span></p>
              <p>Ккал <span>00</span></p>
            </div>
          </div>
        </div>
        <a class="change-button">Редактировать базу 𓂃🖊</a>
      </div>
      <div class="third-div-second-div">
        <table>
          <thead>
            <tr>
              <th>Продукт</th>
              <th>Количество</th>
              <th>Белки</th>
              <th>Жиры</th>
              <th>Углеводы</th>
              <th>Ккал</th>
            </tr>
          </thead>
          <tbody>
            <tr class="tr-1">
              <td style="border-top-left-radius: 5px; border-bottom-left-radius: 5px" class="td-1">
                Куриная грудка <span>🗑️</span>
              </td>
              <td class="td-1 td-h">400</td>
              <td class="td-1 td-h">75</td>
              <td class="td-1 td-h">1,4</td>
              <td class="td-1 td-h">00</td>
              <td
                style="border-top-right-radius: 5px; border-bottom-right-radius: 5px"
                class="td-1"
              >
                444
              </td>
            </tr>
            <tr class="tr-2">
              <td style="border-top-left-radius: 5px; border-bottom-left-radius: 5px" class="td-2">
                Наименование продукта
              </td>
              <td class="td-2 td-h">00</td>
              <td class="td-2 td-h">00</td>
              <td class="td-2 td-h">00</td>
              <td class="td-2 td-h">00</td>
              <td
                style="border-top-right-radius: 5px; border-bottom-right-radius: 10px"
                class="td-2"
              >
                00
              </td>
            </tr>
          </tbody>
        </table>
        <button>Добавить продукт</button>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 10px;

  h1 {
    font-weight: 800;
    font-size: 48px;
    color: white;
  }

  .first-div {
    width: 100%;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: start;
    background-color: #1e242e;
    padding: 50px 60px 50px 60px;
    h2 {
      font-weight: 700;
      font-size: 24px;
      color: white;
      margin-bottom: 32px;
    }

    .first-div-form {
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 20px;
      flex-direction: column;

      .form-first-div {
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 24px;

        div {
          width: 100%;
          display: flex;
          justify-content: center;
          align-items: start;
          gap: 12px;
          flex-direction: column;

          label {
            font-weight: 500;
            font-size: 16;
            color: #9aaac3;
          }

          input {
            width: 100%;
            height: 54px;
            border-radius: 8px;
            padding: 15px 24px 15px 24px;
            background-color: #4f5a6b;
            border: none;
            outline: none;
            color: white;
            font-weight: 400;
            font-size: 18px;
          }

          input::placeholder {
            color: #9aaac3;
            font-weight: 400;
            font-size: 18px;
          }
        }
      }

      .form-second-div {
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 20px;
        div {
          display: flex;
          justify-content: center;
          align-items: center;
          gap: 9px;

          label {
            color: white;
            font-weight: 400;
            font-size: 18px;
          }

          input {
            width: 72px;
            height: 54px;
            border-radius: 8px;
            background-color: black;
            padding: 15px 25px 15px 25px;
            outline: none;
            border: none;
            font-weight: 700;
            font-size: 18px;
            color: white;
          }

          input::placeholder {
            font-weight: 700;
            font-size: 18px;
            color: #9aaac3;
          }
        }

        button {
          width: 300px;
          height: 54px;
          border-radius: 8px;
          border: 2px solid #3b4555;
          background-color: transparent;
          font-weight: 400;
          font-size: 18px;
          color: #9aaac3;
          cursor: pointer;
        }
      }
    }
  }

  .second-div {
    width: 100%;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: start;
    background-color: #1e242e;
    padding: 50px 60px 50px 60px;
    h2 {
      font-weight: 700;
      font-size: 24px;
      color: white;
      margin-bottom: 32px;
    }

    .second-div-form {
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 20px;
      flex-direction: column;

      .form-first-div {
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: end;
        gap: 24px;
        .form-first-div-first-div {
          width: 100%;
          display: flex;
          justify-content: center;
          align-items: center;
          gap: 24px;
          div {
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: start;
            gap: 12px;
            flex-direction: column;

            label {
              font-weight: 500;
              font-size: 16;
              color: #9aaac3;
            }

            input {
              width: 100%;
              height: 54px;
              border-radius: 8px;
              padding: 15px 24px 15px 24px;
              background-color: #4f5a6b;
              border: none;
              outline: none;
              color: white;
              font-weight: 400;
              font-size: 18px;
            }

            input::placeholder {
              color: #9aaac3;
              font-weight: 400;
              font-size: 18px;
            }
          }
        }

        .form-first-div-last-div {
          width: 100%;
          border-radius: 8px;
          background-color: #2c3441;
          padding: 16px 20px 16px 20px;
          display: flex;
          justify-content: center;
          align-items: start;
          gap: 10px;
          flex-direction: column;
          p {
            font-weight: 400;
            font-size: 14px;
            color: #9aaac3;
          }
        }
      }
      .form-second-div {
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 30px;
        div {
          width: 100%;
          display: flex;
          justify-content: space-between;
          align-items: center;
          text-align: left;
          p {
            font-weight: 600;
            font-size: 18px;
          }
          h4 {
            font-weight: 400;
            font-size: 48px;
            color: white;
            white-space: nowrap;
            span {
              font-size: 40px;
            }
          }
        }
      }
    }
  }

  .third-div {
    width: 100%;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: start;
    background-color: #1e242e;
    padding: 50px 60px 50px 60px;

    h2 {
      font-weight: 700;
      font-size: 24px;
      color: white;
      margin-bottom: 32px;
    }

    .third-div-first-div {
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: end;
      gap: 20px;
      flex-direction: column;

      .third-div-form {
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 24px;
        div {
          display: flex;
          justify-content: center;
          align-items: start;
          gap: 12px;
          flex-direction: column;

          label {
            font-weight: 500;
            font-size: 16;
            color: #9aaac3;
          }

          input {
            width: 100%;
            height: 54px;
            border-radius: 8px;
            padding: 15px 24px 15px 24px;
            background-color: #4f5a6b;
            border: none;
            outline: none;
            color: white;
            font-weight: 400;
            font-size: 18px;
          }

          input::placeholder {
            color: #9aaac3;
            font-weight: 400;
            font-size: 18px;
          }
        }
      }

      div {
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 24px;
        .third-div-min-first {
          display: flex;
          justify-content: center;
          align-items: start;
          gap: 12px;
          flex-direction: column;
          width: 100%;
          border-radius: 8px;
          background-color: #55863e;
          padding: 15px 20px 15px 20px;
          h3 {
            font-weight: 500;
            font-size: 18px;
            color: white;
          }
          div {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;
            p {
              font-weight: 400;
              font-size: 16px;
              color: #a2c39a;
              span {
                font-size: 22px;
                color: white;
              }
            }
          }
        }
        .third-div-min-second {
          display: flex;
          justify-content: center;
          align-items: start;
          gap: 12px;
          flex-direction: column;
          width: 100%;
          border-radius: 8px;
          background-color: #2c3441;
          padding: 15px 20px 15px 20px;
          h3 {
            font-weight: 500;
            font-size: 18px;
            color: white;
          }
          div {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;
            p {
              font-weight: 400;
              font-size: 16px;
              color: #9aaac3;
              span {
                font-size: 22px;
                color: white;
              }
            }
          }
        }
      }

      .change-button {
        text-decoration: none;
        font-weight: 400;
        font-size: 16px;
        color: #c6cfde;
        cursor: pointer;
      }
      .change-button:hover {
        background: none;
      }
    }
    .third-div-second-div {
      width: 100%;
      margin-top: 20px;
      table {
        width: 100%;
        thead {
          tr {
            th {
              text-align: left;
              font-weight: 400;
              font-size: 18px;
              color: #9aaac3;
              padding-bottom: 10px;
            }
          }
        }
        tbody {
          tr {
            .td-1 {
              font-weight: 400;
              font-size: 18px;
              color: white;
              background-color: #4f5a6b;
              padding: 17px 16px 17px 16px;
            }
            .td-2 {
              font-weight: 400;
              font-size: 18px;
              color: #9aaac3;
              background-color: #4f5a6b;
              padding: 17px 16px 17px 16px;
            }
          }
        }
      }
      button {
        width: 100%;
        height: 54px;
        border-radius: 8px;
        background-color: transparent;
        border: 2px solid #3b4555;
        color: #9aaac3;
        margin-top: 8px;
      }
    }
  }
}

@media (max-width: 1100px) {
  main {
    .second-div {
      .second-div-form {
        .form-first-div {
          justify-content: start;
          align-items: start;
          .form-first-div-first-div {
            flex-direction: column;
            gap: 8px;
          }
        }
        .form-second-div {
          justify-content: start;
          align-items: start;
          div {
            justify-content: start;
            gap: 10px;
            h4 {
              font-size: 35px;
              span {
                font-size: 25px;
              }
            }
          }
        }
      }
    }
    .third-div {
      .third-div-first-div {
        .third-div-form {
          div {
            input {
              padding: 10px 15px;
            }
          }
        }
      }
    }
  }
}

@media (max-width: 992px) {
  main {
    .first-div {
      padding: 35px;
      .first-div-form {
        .form-first-div {
          div {
            input {
              font-size: 14px;
            }
            input::placeholder {
              font-size: 14px;
            }
          }
        }
      }
    }
    .second-div {
      padding: 35px;
      .second-div-form {
        .form-first-div {
          .form-first-div-first-div {
            div {
              input {
                font-size: 14px;
              }
              input::placeholder {
                font-size: 14px;
              }
            }
          }
        }
        .form-second-div {
          div {
            p {
              font-size: 14px;
            }
            h4 {
              font-size: 25px;
              span {
                font-size: 20px;
              }
            }
          }
        }
      }
    }
    .third-div {
      padding: 35px;
      .third-div-first-div {
        .third-div-form {
          align-items: end;
          div {
            input {
              font-size: 14px;
            }
            input::placeholder {
              font-size: 14px;
            }
          }
        }
      }
    }
  }
}

@media (max-width: 768px) {
  main {
    .first-div {
      .first-div-form {
        .form-first-div {
          gap: 8px;
          div {
            input {
              padding: 6px 12px;
            }
          }
        }
      }
    }
    .second-div {
      .second-div-form {
        .form-first-div {
          flex-direction: column;
        }
        .form-second-div {
          flex-direction: column;
          div {
            justify-content: space-between;
          }
        }
      }
    }
    .third-div {
      .third-div-first-div {
        .third-div-form {
          gap: 8px;
          div {
            input {
              padding: 6px;
            }
          }
        }
        div {
          flex-direction: column;
          .third-div-min-first,
          .third-div-min-second {
            div {
              flex-direction: row;
            }
          }
        }
      }
      .third-div-second-div {
        table {
          thead {
            display: none;
          }
          tbody {
            .tr-1,
            .tr-2 {
              .td-h {
                display: none;
              }
            }
          }
        }
      }
    }
  }
}
</style>
